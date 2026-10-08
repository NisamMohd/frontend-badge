# Day-5

## Async Redux (API Handling)

### createAsyncThunk
    - "createAsyncThunk is a function from Redux Toolkit used to handle asynchronous logic such as API calls."
    - It accepts an action type prefix (e.g., 'users/fetchUsers') and a payload creator callback function that returns a Promise.
    - It automatically generates and dispatches three action types based on the promise lifecycle: pending, fulfilled, and rejected.
    - It provides a `thunkAPI` object which gives access to `dispatch`, `getState`, `rejectWithValue`, and `signal`.

    - createAsyncThunk is a Redux Toolkit utility used to handle asynchronous operations, such as API calls.
    - Instead of manually creating separate actions for loading, success, and failure, createAsyncThunk automatically generates three action states:
        - pending → API request started
        - fulfilled → API request succeeded
        - rejected → API request failed

### Pending / Fulfilled / Rejected States
    - createAsyncThunk automatically generates three lifecycle actions:
        1. pending: Dispatched immediately when the async operation starts (used to set loading = true).
        2. fulfilled: Dispatched when the Promise resolves successfully (used to save data and set loading = false).
        3. rejected: Dispatched when the Promise rejects or throws an error (used to store error message and set loading = false).
    - These actions are handled in the slice using `extraReducers` with the builder callback notation (`builder.addCase()`).

    

### Loading & Error Handling
    - In Redux, we typically manage asynchronous status using state properties like:
        - `loading`: boolean (or `status`: 'idle' | 'loading' | 'succeeded' | 'failed')
        - `error`: null | string
    - Best practices for error handling:
        - Use `rejectWithValue(error.response?.data || error.message)` inside the payload creator so the error payload is passed to the `rejected` action instead of throwing an unhandled exception.
        - Handle UI states cleanly in components: display loaders/skeletons during `loading`, and show alert messages or fallback UI when `error` exists.

### Normalized State
    - "Normalized state means structuring Redux store data like a relational database: flat instead of deeply nested, with entities indexed by their IDs."
    - Key structure:
        - `ids`: An array of all entity IDs (maintains sorting/ordering).
        - `entities`: An object lookup table where keys are IDs and values are entity objects (`{ [id]: item }`).
    - Why normalize state?
        1. Prevents duplicate data across different parts of the state.
        2. Fast lookups: Accessing an item by ID is O(1) instead of searching an array with O(n).
        3. Simple updates: Updating an entity in one place automatically reflects everywhere it is referenced.
        4. Performance: Prevents unnecessary component re-renders.
    - Redux Toolkit provides `createEntityAdapter` to automate and simplify normalized state management.

    "Normalized state is a way of structuring Redux data so that each entity is stored only once, usually indexed by its ID. This reduces duplication, makes updates easier, and is especially useful when working with related or nested entities."