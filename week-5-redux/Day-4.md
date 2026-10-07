# Day-4

## Redux in React Apps

### React-Redux Setup
    - React-Redux is the official library that connects a React application with Redux.
    - The basic setup is:
        npm install @reduxjs/toolkit react-redux

### Provider
    - Provider makes the Redux store available to the entire React component tree.
    - Provider uses React Context internally to make the Redux store accessible to React components.
    - Without Provider, hooks such as useSelector() and useDispatch() cannot access the Redux store.

### useSelector()
    - useSelector() is used to read data from the Redux store.
    - useSelector() subscribes the component to the selected part of the Redux store. When that selected value changes, React-Redux can re-render the component.

### useDispatch()
    - useDispatch() is used to dispatch actions to Redux.

### Multiple Reducers
    - In a real application, we normally have different pieces of state.
    - Multiple reducers allow us to organize Redux state by feature instead of putting all application logic into one large reducer.

### Redux DevTools
    Redux DevTools is a debugging tool used to inspect Redux state changes and actions.
    With Redux Toolkit, DevTools integration is enabled by default when you use configureStore() in development-oriented setups.
