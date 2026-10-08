# Day-6

## TanStack Query Fundamentals

### Server state vs client state

    Server state is data that comes from an external server/API and needs to be synchronized with the backend.

    Server state usually has concerns like loading, caching, refetching, stale data, retries, and synchronization.

    Client state is data that belongs to the UI/application itself.

### useQuery
    useQuery is a TanStack Query hook used to fetch and manage server data.

    TanStack Query handles things such as:
        - Fetching
        - Loading state
        - Error state
        - Caching
        - Refetching
        - Stale data
        - Request deduplication

### useMutation
    useMutation is used when I want to change server-side data.
    Typical operations are:
        - POST
        - PUT
        - PATCH
        - DELETE

### note
    useQuery is mainly for reading/fetching server data.
    useMutation is for creating, updating, or deleting server data.

### Query Keys
    A query key uniquely identifies a piece of server state in the TanStack Query cache.

    The query key is important because TanStack Query uses it to determine:
        - Which cached data belongs to which query
        - Whether two queries represent the same data
        - Which query should be refetched or invalidated

### Cache Concepts
    The cache is where TanStack Query stores previously fetched server data.

    TanStack Query can use the cached result instead of unnecessarily starting another request.

    staleTime — how long fetched data is considered fresh.

    gcTime — how long inactive cached data is retained before garbage collection.