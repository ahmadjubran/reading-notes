# CRUD

## In your own words, describe what each group of status code represents

- 100’s = Informational status codes, these are used to inform the client that the request was received and understood.
- 200’s = Success codes, these are used to inform the client that the request was successfully received, understood, and accepted.
- 300’s = Redirection codes, these are used to inform the client that the resource they are requesting isn’t available at the expected location anymore.
- 400’s = Client error codes, these are used to inform the client that there was a problem with their request.
- 500’s = Server error codes, these are used to inform the client that there was a problem with the server.

## What is a status code 202?

Accepted, this code tells the client that the request has been accepted for processing, but the processing has not been completed.

## What is a status code 308?

Permanent Redirect, this code tells the client that the resource they are requesting has been moved permanently to a new location.

## What code would you use if an update didn’t return data to a client?

204 No Content

## What code would you use if a resource used to exist but no longer does?

410 Gone

## What is the ‘Forbidden’ status code?

403 Forbidden, this code tells the client that the server is refusing to fulfill the request.

## Why do we need to pull our MongoDB database string out of our server and put it into our .env?

So that we can hide our database string from the public.

## What is middleware?

Middleware is software that provides common services and capabilities to applications outside of what’s offered by the operating system.

## What does app.use(express.json()) do?

This is a built-in middleware function in Express. It parses incoming requests with JSON payloads and is based on body-parser.

## What does the /:id mean in a route?

This is a parameter, it is used to capture the value of whatever we specify after the “/”.

## What is the difference beween PUT and PATCH?

PUT is used to update a resource, and PATCH is used to modify a resource.

## How do you make a defalut value in a schema?

You can use the default property.

## What does a 500 error status code mean?

Internal Server Error, this code tells the client that the server encountered an unexpected condition that prevented it from fulfilling the request.

## What is the difference between a status 200 and a status 201?

- 200 OK, this code tells the client that the request has succeeded.
- 201 Created, this code tells the client that the request has succeeded and has led to the creation of a new resource.
