# React Router Catch-All Route Conflict

This repository demonstrates a common issue in React Router v6 where a catch-all route (`/*`) interferes with other defined routes.  The `/*` route, intended to handle 404 errors, matches *before* other routes, even if those routes are more specific.

The solution involves re-ordering the routes to ensure that the catch-all route is placed last within the `Routes` component.