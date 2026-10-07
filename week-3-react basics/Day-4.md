# Day-4

### List vs Key
    In React, a list is used to render multiple elements dynamically, usually using the map() method. A key is a unique identifier given to each item in that list.

### conditional rendering
    Conditional rendering means rendering different UI elements based on a condition.

    React commonly uses if, the ternary operator, and the logical AND (&&) operator.

### Event Handling
    Event handling in React is used to respond to user actions such as clicks, typing, submitting forms, and mouse events.
    React uses camelCase event names and passes a function as the event handler.

    React uses a normalized event system so event handling behaves consistently across browsers.

### Previous state in useState()
    When the new state depends on the previous state, I use the functional updater form of setState.

    Interview point: Whenever the next state depends on the previous state, the functional updater is the safer and recommended approach.

### Form Validation
    Form validation means checking user input before submitting the form to ensure the data satisfies the required rules.
    For example, I might validate:
    - Required fields
    - Email format
    - Password length
    - Password confirmation
    - Minimum/maximum values

    Client-side validation improves user experience, but it should not be treated as a security boundary. Server-side validation is still required because client-side validation can be bypassed.