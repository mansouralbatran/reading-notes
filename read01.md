# Component-Based Architecture
![image](https://www.techdiagonal.com/wp-content/uploads/2019/08/React-components-blog-image.jpg)

## What is a Component?
A component is a modular, portable, replaceable, and reusable set of well-defined functionality that encapsulates its implementation and exporting it as a higher-level interface
## Component-Level Design Guidelines
* Attains architectural component names from the problem domain and ensures that they have meaning to all stakeholders who view the architectural model.

* Extracts the business process entities that can exist independently without any associated dependency on other entities.

* Recognizes and discover these independent entities as new components.

* Uses infrastructure component names that reflect their implementation-specific meaning.

* Models any dependencies from left to right and inheritance from top (base class) to bottom (derived classes).

* Model any component dependencies as interfaces rather than representing them as a direct component-to-component dependency


# What is Props?


![image](https://www.techdiagonal.com/wp-content/uploads/2019/09/react-props-blog-image-design-2.jpg)

React is a component-based library which divides the UI into little reusable pieces. In some cases, those components need to communicate (send data to each other) and the way to pass data between components is by using props.
“Props” is a special keyword in React, which stands for properties and is being used for passing data from one component to another.
But the important part here is that data with props are being passed in a uni-directional flow. (one way from parent to child)



## Using Props in React
* I will be explaining how to use Props step by step.
1. Firstly, define an attribute and its value(data)
2. Then pass it to child component(s) by using Props
2. Finally, render the Props Data