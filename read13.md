## Which HTTP Status Code to Use for Every CRUD App
The HTTP specification defines many status codes we can use when responding to our clients. Some APIs only use the most basic codes and define their own error signaling mechanisms on top of it; others want to make full use of HTTPs collection of codes to tell their clients what’s going on. If you belong to the latter, this article is for you. This guide walks through the various CRUD operations and which status codes you should be using for clean API design.

* HTTP Status CodesPermalink
A status code is a number higher than 100 and smaller than 600 that is part of a HTTP response. The first digit defines the class of the status. A status code comes with a reason phrase. The code is for programmatic recognition the phrase is for humans to understand what happened.

Every status code has to follow these two rules, even custom ones (yes the status codes are extensible).

* Status Classes
If we understand the class a status code is in, we can locate problems more quickly.

## CRUD (Create, Read, Update, Delete)Permalink
## CREATE
The create action is usually implemented via HTTPs POST method. In RESTful APIs, these endpoints are used to create new resources or access tokens.
200 OK - It’s the basic status code to tell the client everything went good. Since we don’t create endpoint accessible resource when creating an access token, we can use 200 as a status for that action.
201 Created - The most fitting for Create operations. This code should signal backend-side resource creation and come along with a Location header that defines the most specific URL for that newly created resource. It’s also a good idea to include appropriate representation of the resource or at least one or more URLs to that resource in the response body.
202 Accepted - Often used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime in the future. The response body should include an URL to the finished resource with some information about when it will be available, or an URL to some monitoring endpoint that tells the client when the resource is available.
303 See Other - Like the 202 code but using a Location header field in response to informing the client about the location of the created resource or an endpoint that lets the client check for the status of the creation process. Some clients follow the status codes of the Redirect-class automatically. This code is usually only used for POST requests.
## READPermalink
The read action gets implemented via HTTPs GET method and used to fetch resource representations. Asynchronous responses aren’t much of a thing here, because the reason for asynchronous processing is often that the resource doesn’t exist yet and has to be created, so it’s a create action anyway.