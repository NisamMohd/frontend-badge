# Day-4

### Lazy loading
    "Lazy loading is a performance optimization where resources are loaded only when they're required. In React, I commonly implement it using React.lazy() and Suspense to achieve code splitting. For example, instead of loading every page in the initial JavaScript bundle, I can dynamically import pages and load their chunks when the user navigates to them. This reduces the initial bundle size and can improve application startup performance."

### useMemo
    useMemo is a React Hook used to memoize a computed value. It executes the calculation during rendering and reuses the previous result until one of its dependencies changes

### useCallback
    useCallback is a React Hook that memoizes a function reference. It returns the same function between renders until one of its dependencies changes. It's mainly useful when passing callbacks to memoized child components with React.memo, because without it, a new function reference is created on every parent render and can cause unnecessary child re-renders.

### React.memo()
    React.memo is a higher-order component used to optimize functional components. It memoizes the rendered component and skips re-rendering when its props haven't changed according to shallow comparison. It is useful when a component re-renders frequently with the same props