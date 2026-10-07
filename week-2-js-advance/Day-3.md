# Day-3

### Exception Handling
    “Exception handling in JavaScript is used to handle runtime errors without crashing the application. We generally use try to execute risky code, catch to handle exceptions, finally for cleanup code, and throw to manually generate custom exceptions. JavaScript also provides built-in error types such as TypeError, ReferenceError, SyntaxError, and RangeError.”

    try...catch handles runtime exceptions, not every kind of error. For example, a syntax error in the same script generally prevents that script from being parsed and executed in the first place.

    1. try
    The try block contains code that might produce an exception.

    2. catch
    The catch block executes when an exception occurs inside try.

    3. finally
    The finally block executes whether an exception occurs or not.

    4. throw
    We can manually generate an exception using throw.

### async & await
    “Async and await are JavaScript features used to handle Promise-based asynchronous operations. The async keyword makes a function return a Promise, while await pauses the execution of that async function until the Promise settles. It doesn't block the main JavaScript thread. We commonly use try...catch with async/await for error handling, and Promise.all() when multiple independent asynchronous operations need to run concurrently.”