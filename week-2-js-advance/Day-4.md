# Day 4

### Object & Class
    An object is an individual entity that contains properties and methods. A class is a blueprint or template used to create multiple objects with the same structure and behavior.

### Instance
    An instance is an object created from a class using the new keyword.

### Constructor
    A constructor is a special method in a JavaScript class that automatically executes when an object is created using new. It is mainly used to initialize object properties.

### Garbage collection
    Garbage collection is the automatic process of identifying objects that are no longer reachable by a program and reclaiming their memory.

### Shadowing & Illegal Shadowing
    Shadowing occurs when a variable declared in an inner scope has the same name as a variable in an outer scope.

    Illegal shadowing occurs when a declaration conflicts with a lexical declaration in an outer scope in a way JavaScript does not allow.

    Shadowing means an inner variable hides an outer variable with the same name. Illegal shadowing happens when certain var and lexical declarations (let/const/class) conflict in nested scopes.

### Memory leak
    A memory leak occurs when a program unintentionally keeps references to objects that are no longer needed, preventing garbage collection and causing memory usage to grow.

### Allocation and Deallocation
    Memory allocation means reserving memory for data during program execution.

    Deallocation means releasing memory that is no longer required.

    Allocation is the process of reserving memory for data, while deallocation is releasing memory when it is no longer needed. In JavaScript, allocation and reclamation are largely handled automatically by the JavaScript engine and garbage collector.

### Memoization

    Memoization is an optimization technique where the result of an expensive function call is cached so that when the same input occurs again, the cached result can be returned instead of recalculating it.

    Memoization improves performance when computation is expensive and repeated, but it also consumes memory because cached results must be stored. It should not be used automatically for every calculation.