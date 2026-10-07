# Day-5

### Deep Copy & Shallow Copy
    A shallow copy creates a new object, but nested objects or arrays are still referenced from the original object. So, changing a nested value in the copied object can affect the original.

    A deep copy creates a completely independent copy, including nested objects and arrays. Changes to the copied object do not affect the original.

### Weak Set() & Weak Map()
    WeakSet is a collection that stores objects only and holds them weakly, meaning an object can still be garbage-collected if there are no other strong references to it.

    WeakMap stores key-value pairs, where the keys must be objects and are held weakly.

### Optional Chaining (?.) vs Nullish coalescing
    It safely accesses a property or method when the value before ?. may be null or undefined.

    ?? provides a default value only when the left side is null or undefined.

    Optional chaining prevents errors when accessing potentially null or undefined properties, while nullish coalescing provides a fallback specifically for null or undefined values.

### Debouncing and Throttling
    Both are techniques for controlling how frequently a function executes when an event occurs repeatedly.

    Debouncing delays function execution until the user stops triggering the event for a specified amount of time.

    Throttling ensures that a function executes at most once during a specified time interval, even if the event happens continuously.