# Routes

Holism supports single-level routing. However, it does not support nested routes.

### Module routes
Each module can have its own routes.

Inside the `Admin` directory of the module, create a file called `Exports.jsx`.

Inside that file create an array of routes and export it as a named export:

```
const BlogRoutes = [
    // routing rules
]

export { BlogRoutes }
```

