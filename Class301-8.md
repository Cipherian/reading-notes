# This is my journal 8/09/2022

## What does REST stand for?

- Representational State Transfer

## REST APIs are designed around a ____.

> REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client.

## What is an identifier of a resource? Give an example.

> A resource has an identifier, which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be: https://adventure-works.com/orders/1

## What are the most common HTTP verbs?

- GET, POST, PUT, PATCH, and DELETE.

## What should the URIs be based on?

- URIs should be based on nouns

## Give an example of a good URI.

- Knight, order, chicken

## What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

- Chatty apis have too many server requests. Therefore, try to avoid "chatty" web APIs that expose a large number of small resources.

## What status code does a successful GET request return?

- GET retrieves a representation of the resource at the specified URI. The body of the response message contains the details of the requested resource.

## What status code does an unsuccessful GET request return?

- 204 (no content)

## What status code does a successful POST request return?

- POST creates a new resource at the specified URI. The body of the request message provides the details of the new resource. Note that POST can also be used to trigger operations that don't actually create resources.

## What status code does a successful DELETE request return?

- DELETE removes the resource at the specified URI.

- Source: 