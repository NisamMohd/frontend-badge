# Day-2

## Redux Core Concepts

### Redux Architecture Overview
    Redux is a predictable state management library used to manage application-wide state.
    The core architecture consists of:
    - Store → holds the application state.
    - Action → describes what happened.
    - Reducer → determines how the state should change.
    - Dispatch → sends an action to the Redux store.
    - Selector → reads required data from the store.
    The important principle is that state changes are centralized and predictable.

### Store, Actions, Reducers
    The store is the central container that holds the application's Redux state.

    An action describes an event that happened in the application.

    A reducer is a function that determines the new state based on the current state and the dispatched action.

### Immutable Updates
    "Redux requires immutable state updates conceptually. With Redux Toolkit, Immer allows us to write mutation-like syntax while producing immutable state updates internally."

### single source of truth
    "Not every piece of state belongs in Redux. Local UI state such as whether a dropdown is open can usually remain inside the component."
    The application's shared Redux state is maintained in one centralized store.

### Redux Flow
    "Redux follows a unidirectional data flow architecture. The application has a centralized store that contains the shared state. When something happens in the UI, we dispatch an action describing that event. The action goes to the reducer, and the reducer calculates the new state from the previous state and the action. Redux then updates the store with the new state, and the components that depend on that state re-render. Redux follows immutable updates and provides a single source of truth for shared application state."