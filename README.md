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
