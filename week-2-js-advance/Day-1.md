# Day-1

## Synchronous & Asynchronous

    “Synchronous JavaScript executes code one statement at a time, in sequence. Each operation must finish before the next operation starts, so it can block the execution.
    Asynchronous JavaScript allows certain long-running operations, such as API calls, timers, or file operations, to be handled without blocking the main JavaScript thread. Once the operation completes, its callback or Promise continuation is scheduled to run.”

## Js execution
    “JavaScript executes code inside an execution context. The execution context contains the information required to run the code, such as variables, functions, and the this value. JavaScript uses a call stack to manage execution. For asynchronous operations, the event loop coordinates between the call stack and task or microtask queues.”
### Execution Context
    An Execution Context is the environment in which JavaScript code is evaluated and executed.
    There are mainly three types:
    1. Global Execution Context
    2. Function Execution Context
    3. Eval Execution Context — rarely used in normal development.
#### Global Execution Context
#### Function Execution Context
#### Eval Execution Context — rarely used in normal development.

### Event Loop
    “The event loop does not execute JavaScript itself. It coordinates when queued callbacks can be moved onto the call stack.”

### Call Stack
    The Call Stack is a LIFO data structure used by JavaScript to keep track of currently executing functions.
### Overflow & Underflow
    “Stack overflow occurs when the call stack grows beyond its maximum supported size, commonly because of infinite or excessively deep recursion.”

    “Stack underflow means trying to pop from an empty stack. In JavaScript's built-in execution call stack, this is managed internally by the engine, so developers normally encounter stack overflow rather than call-stack underflow.”

## Hoisting
    “Hoisting is JavaScript's behavior where declarations are processed during the creation phase of an execution context before the code is executed. However, different declarations are initialized differently, so hoisting does not mean that the actual code is physically moved to the top.”

    “Hoisting is the JavaScript behavior where declarations are processed during execution-context creation before normal code execution. var is initialized to undefined, while function declarations are initialized with their function definition.”

## Temporal Dead Zone

    “TDZ is the period between entering a scope and the initialization of a let, const, or class binding. Accessing that binding during the TDZ throws a ReferenceError.”