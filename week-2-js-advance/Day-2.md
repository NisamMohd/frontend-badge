# Day  2

### Fetch API
    “Fetch API is a built-in JavaScript API used to make HTTP requests such as GET, POST, PUT, PATCH, and DELETE. It is promise-based, so it is commonly used with .then(), .catch(), or async/await.”

### Promise
    “A Promise is an object that represents the eventual completion or failure of an asynchronous operation.”
    A Promise has three states:
    1. Pending – operation is still running.
    2. Fulfilled – operation completed successfully.
    3. Rejected – operation failed.

####  promise  methods
    .then() — handles successful fulfillment. 

    .catch() — handles rejection/errors.

    .finally() — executes regardless of success or failure.

    Promise.all - Runs multiple promises and waits for all of them.

    Promise.allSettled() - Waits for every Promise, regardless of whether it succeeds or fails.

    Promise.race() - Returns the first Promise that settles — fulfilled or rejected.

    Promise.any() - Returns the first Promise that fulfills.If all promises reject, it rejects with an AggregateError


### callback hell
    “Callback hell occurs when multiple asynchronous operations are nested inside callbacks, making the code difficult to read, maintain, and handle errors in.”

    Problems:
    - Poor readability
    - Difficult debugging
    - Difficult error handling
    - Difficult maintenance
    - Deep nesting
    How do we avoid callback hell?
    The modern solutions are Promises and async/await.

    Interview one-liner:
    “Callback hell is excessive nesting of callbacks. Promises and async/await provide a cleaner way to manage asynchronous operations.”

### JSON
    “JSON stands for JavaScript Object Notation. It is a lightweight text-based data format commonly used for exchanging data between a client and a server.”

    JSON.stringify()
    Converts a JavaScript object into a JSON string.

    JSON.parse()
    Converts a JSON string into a JavaScript value.

    JSON is a text/data format. After JSON.parse(), the JSON text becomes a JavaScript value such as an object or array.

    