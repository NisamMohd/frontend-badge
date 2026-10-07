# Day-4

## Iteration Methods
### array.map()
    map() is used when I want to transform every element of an array. It returns a new array with the same number of elements.

    Interview point: map() returns a new array and does not modify the original array.

### array.filter()
    filter() is used when I want to select elements based on a condition. It returns a new array containing only the elements for which the callback returns true.

    Interview point: filter() can return fewer elements than the original array, including an empty array.

### array.reduce()
    reduce() is used when I want to reduce an array to a single value. That value could be a number, string, object, array, etc.

    Interview point: reduce() is commonly used for sums, averages, grouping, counting, and converting arrays into objects.

### array.forEach()
    forEach() is used when I simply want to execute some operation for each element. It does not return a new array.

    Interview point: forEach() returns undefined, so I cannot directly use it for creating a transformed array

## JS DOM
### JS HTML DOM
    DOM stands for Document Object Model. It is a programming interface provided by the browser that represents an HTML document as a tree of objects. JavaScript can use the DOM to access, modify, create, or delete HTML elements, CSS styles, attributes, and event handlers dynamically.

### DOM Intro
    - The browser converts HTML into a DOM tree.
    - Each HTML element becomes a DOM element/node object that JavaScript can manipulate.
    - HTML is the source markup, while DOM is the browser's object representation of that markup
### DOM Methods
    DOM methods are JavaScript functions used to find, create, modify, or remove elements

### DOM Document
    - document represents the entire HTML page.
    - The document object is the entry point for accessing and manipulating the DOM.

### DOM Elements
    - An HTML element in the DOM can be accessed and manipulated using JavaScript.

### DOM HTML
    - JavaScript can modify the HTML/content inside an element.

### DOM CSS
    JavaScript can dynamically change CSS.

### DOM Events
    An event is an action that happens in the browser.

### DOM Event Listener

