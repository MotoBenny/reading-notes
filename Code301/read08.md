# Read08

## [Api design and best practices](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)

What does REST stand for?

Representational State Transfer

REST APIs are designed around a ____.

REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client.

What is an identifer of a resource? Give an example.

A resource has an identifier, which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:

What are the most common HTTP verbs?

The most common operations are GET, POST, PUT, PATCH, and DELETE

What should the URIs be based on?

A unique resource.

Give an example of a good URI.

https://Bens-Portfolio.com/Purchase/01

What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

Chatty API means your APO is making lots of web requests. this imposes needless load on the server, Its a bad thing.

What status code does a successful GET request return?

A successful GET method typically returns HTTP status code 200 (OK).

What status code does an unsuccessful GET request return?

If the resource cannot be found, the method should return 404 (Not Found).



What status code does a successful POST request return?

if a POST method creates a new resource, it returns HTTP status code 201 (Created).

What status code does a successful DELETE request return?

If the delete operation is successful, the web server should respond with HTTP status code 204 (No Content)
