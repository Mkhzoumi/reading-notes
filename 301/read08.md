
# RESTful web API design

## What does REST stand for?
+ ## REST is an architectural style for building distributed systems based on hypermedia. 

## REST APIs are designed around a ____.
+ ## REST APIs are designed around resources.

## What is an identifer of a resource? Give an example.
+ ## a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:

```
https://adventure-works.com/orders/1
```

## What are the most common HTTP verbs?
+ ##  The most common operations are GET, POST, PUT, PATCH, and DELETE.

## What should the URIs be based on?
+ ##  URIs should be based on nouns (the resource) 
## Give an example of a good URI.

```
https://adventure-works.com/orders // Good

https://adventure-works.com/create-order // Avoid
```

## What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
+ ##  "chatty" web APIs that expose a large number of small resources. its a bad thing and you should avoid.

## What status code does a successful GET request return?
+ ## A successful GET method typically returns HTTP status code 200 (OK).

## What status code does an unsuccessful GET request return?
+ ## return 404 (Not Found).

## What status code does a successful POST request return?
+ ##  it returns HTTP status code 201 (Created).

## What status code does a successful DELETE request return?
+ ## HTTP status code 204.









# [back](../README.md)