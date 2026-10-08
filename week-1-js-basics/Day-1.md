# week-1

## Day-1

### what is java script
    - high-level : manage memory or h/w directly,the engine handles memmory through garbage collection
    - interpreted : code isn't compiled ahead of time into a standalone binary.compile hot code paths to machine code at runtime for speed
    - dynamically typed : variable types are determined at run time,not declared up front.
    - multi-paradigm : it supports procedural,object-oriented(prototype-based) and functional proghramming styles
    - single threded : one call stack executes one piece of code at a time
    - used to make pages inteeractive(client-side)
    - runs servers and handlebackend through node.js
    - 

### variables
    - a named container or a symbolic name bound to a value stored 
    ○ var - function scoped.hoisted,initialised as undefined
    ○ let - block scope & reassignable,hoisted,not initialized ,(TDZ)
    ○ const - block scoped & cannot re-assign,hoisted,not initialized ,(TDZ)
### Data types
    - data types classifies what kind of value a variable holds and what operations can be performed on it
    ○ Primitive Types
        - immutable : cannot be changed once created and stored by value in the stack/memory location of the variable
        - compared or copied by value
    ○ Non-Primitive (Reference data types)
        - referance type data structure
        - mutable : stored as a reference or a memory address/pointer rather than the actual value
        - comapared or copied by reference

### Operators
    1. Arithmetic Operators
    2. Assignment Operators
    3. Comparison Operators
    4. Logical Operators
    5. Nullish Coalescing (??) — ES2020
    6. Optional Chaining (?.) — ES2020
    7. Ternary Operator
    8. Bitwise Operators
    9. typeof and instanceof

### Coercion or Type conversion
    ○ type coercion
        - Implicit Type Coercion (engine-driven)
        - automatic conversion of a value from one data type to another
    ○ type conversion 
        - Explicit Type Conversion (developer-driven)
        - same process of coerecion but done by explicitly by developerusing functions like String(),Number() or Boolean()

### Conditional statements
    If else : 
        "if-else is a decision-making statement. It executes one block when a condition is true and another block when the condition is false."

    Switch case : 
        "switch-case is used for multiple fixed-value comparisons. It checks an expression against different case values and executes the matching block. break prevents fall-through, and default handles cases where there is no match."

    Ternary operator : 
        The ternary operator is a conditional operator in JavaScript that provides a short way to write a simple if-else statement.

### JavaScript Loops
    • For loop
    • while loop
    • do while loop

    "for, while, and do...while are looping statements used to repeatedly execute code. I generally use a for loop when the number of iterations is known. I use a while loop when the number of iterations depends on a condition. A do...while loop is useful when I need the code to execute at least once, because its condition is checked after the loop body."
### Function
    - block of reusable code that takes optional input as parameters,performs an operation, an optionally return an output
    
### Object 
    “An object in JavaScript is a mutable, non-primitive data structure that stores data as key-value pairs and can also contain methods.”

### JS ITERATION    
#### For In loop 
        The for...in loop is used to iterate over the enumerable property keys of an object.

        for...in gives me the keys/indexes, not the values directly.

#### For Of loop
        The for...of loop is used to iterate over the values of an iterable.

        It works with arrays, strings, Sets, Maps, and other iterables.

#### Scopes
    - Scope defines where a variable can be accessed in a JavaScript program.
    - There are mainly three scopes you should know:
        1. Global scope
            A variable declared outside functions and blocks is generally in the global scope.

        2. Function scope
            Variables declared with var inside a function are accessible within that function.

        3. Block scope
            A block is code surrounded by { }, such as an if, for, or while.

        "for...in is mainly used to iterate over the keys or property names of an object, while for...of is used to iterate over the values of an iterable such as an array or string. Scope defines where a variable can be accessed. JavaScript has global, function, and block scopes. var is function-scoped, whereas let and const are block-scoped."


