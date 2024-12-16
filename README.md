# React Router Wildcard Route Issue

This repository demonstrates a common issue with React Router's wildcard route ('*').  The wildcard route, intended to catch all unmatched paths, is unexpectedly overriding more specific routes, preventing access to those routes.

The issue stems from incorrect placement or configuration of the wildcard route within the `Routes` component.  The solution involves carefully ordering and structuring routes to ensure specific routes are checked before the wildcard route.

## How to Reproduce

1. Clone the repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe that navigating to `/about` still shows the 404 page (NotFound component).