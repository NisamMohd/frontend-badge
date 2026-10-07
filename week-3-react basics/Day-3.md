# Day-3

### Hooks
#### useState()
    useState is a React Hook used to store and manage state in a functional component.

#### useEffect()
    useEffect is used to perform side effects in a functional component.

#### useRef()
    useRef is used to store a mutable value that persists between renders without causing a re-render when it changes.

### Life Cycle Methods in useEffect()
    "useEffect() is used to handle side effects in functional components. Depending on its dependency array, it can execute after mounting and when dependencies change. The cleanup function handles resource cleanup, such as removing event listeners, clearing timers, or unsubscribing from subscriptions, both before an effect re-runs and when the component unmounts."

    useEffect() Lifecycle
    In functional components, useEffect() is used to perform side effects such as API calls, subscriptions, timers, event listeners, or DOM-related operations.
    It mainly corresponds to three lifecycle phases:
    1. Mounting — component is created and rendered for the first time.
    2. Updating — component re-renders because state or props change.
    3. Unmounting — component is removed from the DOM.

    1. Mounting
    If I want the effect to run only once after the component mounts, I use an empty dependency array:

    2. Updating
    If I provide dependencies, the effect runs after the initial render and whenever those dependencies change.

    3. Unmounting / Cleanup
    The function returned from useEffect() is called when the component is unmounted.