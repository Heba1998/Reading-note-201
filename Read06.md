# Problem Domain, Objects, and the DOM


## OBJECTS:

![img](https://miro.medium.com/max/2722/1*iKJx57JU9sKdff-Os7upyA.png)

**WHAT IS AN OBJECT?**

*Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. *

![img](https://fireship.io/courses/javascript/img/js-object-props.png)

**In JavaScript, almost everything is an object.**

- Booleans 
- Numbers 
- Strings 
- Dates 
- Maths  
- Arrays 
- Functions 


**How to create object:**

![img](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/07/How-to-Create-JavaScript-Objects.jpg)


### **Create object using an Object Literal:**
This is the easiest way to create a JavaScript Object.
Using an object literal, you both define and create an object in one statement.
An object literal is a list of name:value pairs inside curly braces {}.


## The Document Object Model (DOM):

![IMG](https://cf.ppt-online.org/files/slide/l/lG6hjyFR8carDYH7oVAtPW3exEOg0sSpQ1JKfm/slide-4.jpg)
*As a browser loads a web page, it creates a model of that page.
The model is called a DOM tree, and it is stored in the browsers' memory.
It consists of four main types of nodes.*


**why is it used?**

*to specifies how browsers should create a model of an HTML page and how JavaScript can access and update the
contents of a web page while it is in the browser window.*

**Accessing and updating the DOM tree involves two steps:**
1. Locate the node that represents the element you want to work with.
2. Use its text content, child elements, and attributes. 


***The*** getElementById ***Method The most common way to access an HTML element is to use the id of the element.***

**TRAVERSING THE DOM**
*When you have an element node, you can select
another element in relation to it using these five
properties. This is known as **traversing the DOM.***

1. parentNode

    - This property finds the element node for the containing (or parent) element in the HTML.

2. previousSibling nextSibling
    - These properties find the previous or next sibling of a node if there are siblings .


3. firstChild lastChild
     - These properties find the first or last child of the current element.        





## **HOW TO GET/UPDATE ELEMENT CONTENT?**

*The textContent property sets or returns the text content of the specified node, and all its descendants.*

*If you set the textContent property, any child nodes are removed and replaced by a single Text node containing the specified string.*

- textContent returns the text content of all elements, while innerText returns the content of all elements, except for <**script**> and <**style**> elements.
- innerText will not return the text of elements that are hidden with CSS (textContent will).


**ADDING ELEMENTS USING DOM MANIPULATION**
*DOM manipulation offers another technique
to add new content to a page (rather than
i nnerHTML). It involves three steps:*
1. createEl ement () 
2. createTextNode() 
3. appendChild() 

![IMG](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/08/JavaScript-Document-Object-Model-DOM-1200x720.jpg)

**SUMMARY:**
- The browser represents the page using a DOM tree.
- DOM trees have four types of nodes: document nodes,
element nodes, attribute nodes, and text nodes.
- You can select element nodes by their id or cl ass
attributes, by tag name, or using CSS selector syntax.
- Whenever a DOM query can return more than one
node, it will always return a Nadel i st. 
- From an element node, you can access and update its
content using properties such as textContent and
i nnerHTML or using DOM manipulation techniques.
- An element node can contain multiple text nodes and
child elements that are siblings of each other.
- In older browsers, implementation of the DOM is
inconsistent (and is a popular reason for using jQuery).
- Browsers offer tools for viewing the DOM tree .

