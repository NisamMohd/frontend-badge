# Day-3

## Redux Toolkit (Modern Redux)

### configureStore
    "configureStore is the recommended way to create a Redux store in Redux Toolkit. It automatically configures common middleware, enables DevTools in development, and makes reducer configuration simpler."

### createSlice
    "createSlice is a Redux Toolkit API that combines the reducer logic, initial state, and action creators into a single slice. It automatically generates action creators and action types based on the reducer names."

### createAction
    "createAction creates an action creator and automatically generates the action object with a type and optional payload. Unlike createSlice, it does not create reducers."

### immer
    "Immer is a library used for convenient immutable state updates. It gives us a draft state that we can modify using normal mutation syntax. Immer then detects those changes and produces a new immutable state without modifying the original state. Redux Toolkit uses Immer internally in createSlice and createReducer."
    