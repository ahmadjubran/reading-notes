# APIs

## What does REST stand for?

REpresentational State Transfer

## REST APIs are designed around a ?

resources

## What is an identifier of a resource? Give an example

URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:

    https://adventure-works.com/orders/1

## What are the most common HTTP verbs?

- GET
- POST
- PUT
- PATCH
- DELETE

## What should the URIs be based on?

URIs should be based on nouns (the resource) and not verbs (the operations on the resource).

## Give an example of a good URI

    https://adventure-works.com/orders // Good

## What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

- Chatty API is one that requires consumer to make tremendous (subjective matter) amount of distinct API calls to get needed information about a resource.

- chatty APIs are bad because requiring multiple network calls will slow down an application.

## What status code does a successful GET request return?

HTTP status code 200 (OK).

## What status code does an unsuccessful GET request return?

HTTP status code 404 (Not Found).

## What status code does a successful POST request return?

HTTP status code 200 and include the result of the operation in the response body.

## What status code does a successful DELETE request return?

HTTP status code 204 (No Content)

## Things I want to know more about
