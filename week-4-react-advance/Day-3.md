# Day-3

### React router dom
    react-router-dom is a library used to implement client-side routing in React applications. It allows us to navigate between different components/pages without doing a full browser reload.

#### Dynamic Routing
    Dynamic routing means creating a route where part of the URL is variable. It is useful when we have many similar pages, such as product details, user profiles, or blog posts

    Dynamic routing allows me to use a single route for multiple URLs by defining dynamic parameters such as :id, and I can access those parameters using useParams().

#### useParams
    useParams() is a React Router hook used to access dynamic parameters from the current URL.

    "useParams() is a React Router hook that allows me to access dynamic route parameters from the URL, such as an id in /users/:id."

#### useNavigate
    useNavigate() is a React Router hook that I use when I need to navigate programmatically based on some application logic, such as redirecting after login or form submission

#### Nested Routing
    Nested routing allows me to organize child routes under a parent route and reuse a common layout. React Router uses <Outlet /> in the parent component to render the matched child component.