# RESTful web API design
* Platform independence. Any client should be able to call the API, regardless of how the API is implemented internally. This requires using standard protocols, and having a mechanism whereby the client and the web service can agree on the format of the data to exchange.

* Service evolution. The web API should be able to evolve and add functionality independently from client applications. As the API evolves, existing client applications should continue to function without modification. All functionality should be discoverable so that client applications can fully use it.
## What is REST?
* REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client.

* A resource has an identifier, which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be
* REST APIs use a uniform interface, which helps to decouple the client and service implementations. For REST APIs built on HTTP, the uniform interface includes using standard HTTP verbs to perform operations on resources. The most common operations are GET, POST, PUT, PATCH, and DELETE.
## Organize the API design around resources
Focus on the business entities that the web API exposes. For example, in an e-commerce system, the primary entities might be customers and orders. Creating an order can be achieved by sending an HTTP POST request that contains the order information. The HTTP response indicates whether the order was placed successfully or not. When possible, resource URIs should be based on nouns (the resource) and not verbs (the operations on the resource)
## Define API operations in terms of HTTP methods
* GET retrieves a representation of the resource at the specified URI. The body of the response message contains the details of the requested resource.
* POST creates a new resource at the specified URI. The body of the request message provides the details of the new resource. Note that POST can also be used to trigger operations that don't actually create resources.
* PUT either creates or replaces the resource at the specified URI. The body of the request message specifies the resource to be created or updated.
* PATCH performs a partial update of a resource. The request body specifies the set of changes to apply to the resource.
* DELETE removes the resource at the specified URI.