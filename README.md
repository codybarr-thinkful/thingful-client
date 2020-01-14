# Thingful Client

Thinkful Module: JWT / Checkpoint 3

## Assignment

For this assignment you'll refactor the thingful-server and thingful-client projects. You'll change the server so that it supports protected endpoints for getting specific things and posting reviews of things.

Requirements

1. Implement a basic authentication middleware to use for protecting endpoints.
1. The GET /api/things endpoint should remain public.
1. The GET /api/things/:thing_id endpoint should be protected by basic auth.
1. The GET /api/things/:thing_id/reviews endpoint should be protected by basic auth.
1. The POST /api/reviews endpoint should be protected by basic auth and automatically assign a user_id.
1. The thingful-client should store the base64 encoded credentials when the login form is submitted.
1. The base64 encoded credentials should be sent in requests to protected endpoints.
1. If a user attempts to view the login form when they're already logged in, they should be redirected to the thing list 1. page.
1. If a user tries to view reviews for a thing, they should be redirected to the login form page.

## Updates

**Checkpoint 4**

-   You should implement the logout button functionality to clear the token in local storage.

**Checkpoint 5**

-   You should update your login form to call the login endpoint and store the JWT from the response in local storage.
-   Ensure that all the API requests use this token instead of the basic token.

**Checkpoint 6**

-   The registration endpoint should appropriately validate the required fields, including unique usernames and complex non-ambiguous passwords.
-   You should store passwords as bcrypted hashes for better data protection.
