# Day-6

## REST Parameter and SPREAD Operator
### Rest Parameter
    The rest parameter allows a function to accept any number of arguments and collect them into a single array.

### Spread Operator
    The spread operator is also written as ..., but instead of collecting values, it expands/unpacks an iterable or object into individual elements/properties.

## Destructuring
### Array destructuring
    Array destructuring is a JavaScript feature that allows me to extract values from an array and assign them to variables in a single statement.

### object destructuring
    Object destructuring allows me to extract properties from an object and assign them to variables.

    Unlike array destructuring, object destructuring works based on property names, not positions.

## JS Object Method
### JS object method using this keyowrd
    An object method is a function stored as a property of an object. Inside that method, this generally refers to the object that is calling the method.

### call, apply and bind method

    call() immediately invokes the function and allows me to specify the this value.

    apply() is almost the same as call(), but it accepts arguments as an array.

    bind() does not immediately execute the function.
    Instead, it returns a new function with this permanently associated with the specified object.

    "call, apply, and bind are Function methods used to explicitly set the this value. call invokes the function immediately with arguments passed individually. apply also invokes it immediately, but arguments are passed as an array. bind does not invoke the function immediately; it returns a new function with this bound to the specified object. A common use of bind is when I need to pass a method as a callback while preserving its this context."

### Recursion
    "Recursion is a technique where a function calls itself to solve a smaller instance of the same problem. Every recursive function should have a base case to terminate the recursion and a recursive case that moves toward that base case. Recursion uses the call stack, so if the base condition is missing or never reached, it can result in a stack overflow.

    