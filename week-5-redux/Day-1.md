# Day-1

## State Management Fundamentals

### What is State Management?
    “State management is the way we store, update, and share data that can change over time in an application. In React, state can be managed locally using useState, or globally using tools like Context API, Redux, Zustand, etc.
    The main purpose of state management is to keep application data predictable, consistent, and accessible to the components that need it.”

### Local vs Global State
    State required by only one component or a small component subtree.

    State that needs to be accessed or modified by multiple unrelated components.

    “I use local state by default. I introduce global state only when multiple parts of the application genuinely need to share and coordinate the same state.”

### Problems with Prop Drilling
    Prop drilling means passing data through intermediate components that don't actually need that data, just so a deeply nested component can receive it.

    Makes component interfaces unnecessarily complicated.
    Creates tight coupling between components.
    Makes refactoring harder.
    Makes deeply nested data flow difficult to understand.
    Can become difficult to maintain in large applications.

    “Prop drilling itself is not always bad. For a small component tree, props are often the simplest and most explicit solution. It becomes a problem when the same data has to travel through many unrelated components.”

### When NOT to Use Redux
    1. State is purely local
    2. Small application :- If an application has very little shared state, Redux can add unnecessary boilerplate and architectural complexity.
    3. Context is sufficient :- Context may be enough, depending on update frequency and application architecture.
    4. The data is server state :- This data usually comes from an API and has concerns such as caching, refetching, stale data, retries, and synchronization. A server-state library such as TanStack Query is often more appropriate

    “I don't use Redux for every piece of state. I use it when the application has complex client-side state that needs centralized management, predictable updates, and sharing across many components.

### Synchronous State vs Asynchronous Server State
    “Client state is owned and controlled by the frontend, while server state is owned by the backend and only cached or synchronized by the frontend. Redux is commonly used for complex client state, while TanStack Query is designed specifically for server state.”

### Why Redux + TanStack Query together?
    “Redux and TanStack Query solve different state-management problems. Redux is primarily useful for complex client-side state that needs centralized and predictable updates. TanStack Query is designed for server state and handles caching, synchronization, refetching, loading, errors, and stale data. So I wouldn't normally store API responses in Redux just to manage them manually when TanStack Query can handle those concerns. Using both can give a clean separation between client state and server state.