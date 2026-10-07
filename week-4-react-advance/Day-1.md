# Day-1

### JSON Server
    JSON Server is a mock REST API server that uses a JSON file as a database and automatically provides CRUD endpoints, which is useful for frontend development and API prototyping.

### Pagination
    Pagination is used to improve application performance by fetching data in smaller chunks. I usually send the page number and page size to the API, and the backend returns only that portion of the data

### POST, PUT, PATCH, DELETE & GET (JSON)
    "GET is used to retrieve data from the server. It should not be used to modify server-side data."

    "POST is used to create a new resource. The data is usually sent in the request body as JSON."

    "PUT is generally used to replace the complete resource. If I use PUT, I normally send the complete representation of the resource."

    "PATCH is used for partial updates. If I only need to change one or a few fields, PATCH is more appropriate than replacing the entire resource."

    "DELETE is used to remove a resource from the server."

### axios
    Axios is a promise-based HTTP client that I use to communicate with REST APIs. It supports methods like GET, POST, PUT, PATCH, and DELETE and provides features such as request and response interceptors, automatic JSON handling, and centralized configuration."