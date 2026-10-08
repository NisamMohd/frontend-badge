# Day-7

## Advanced TanStack Query

### Pagination with useQuery
    Pagination means fetching data page by page instead of loading all records at once.
    With TanStack Query, I include the page number in the query key.

    "I put pagination parameters in the query key so TanStack Query can cache and manage each page independently."

### Dependent Queries
    A dependent query is a query that should execute only after another query has produced some required data.

    "I use the enabled option to control whether a query should execute. This is useful when one API request depends on the result of another."

### Optimistic Updates
    An optimistic update means updating the UI immediately before the server confirms the operation.

    "Optimistic updates improve perceived performance by updating the cache immediately. If the mutation fails, I roll back the cached data and refetch to synchronize with the server."

### Query Invalidation
    Query invalidation tells TanStack Query that cached data may be stale.

    "I use query invalidation to tell TanStack Query that cached data is no longer fresh. This prompts TanStack Query to refetch the data from the server when the query is next accessed." 

    Invalidation does not simply mean deleting the cache.
    It marks matching queries as stale and can trigger a refetch depending on whether they are active and the query configuration.

    "After a mutation changes server data, I invalidate the affected query so TanStack Query knows its cached data may no longer be valid."

### Prefetching
    Prefetching means loading data before the user actually requests it.

    "I use prefetching when I can predict what data the user is likely to request next. It reduces perceived latency."

### Background Refetch
    TanStack Query can refetch stale data in the background while the application continues displaying cached data.