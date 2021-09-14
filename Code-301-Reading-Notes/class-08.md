## What does REST stand for?
 Representational State Transfer (REST) as an architectural approach
 to designing web services.
 * REST APIs are designed around resources
 * A resource has an identifier
 * Clients interact with a service by exchanging representations of resources. 
 * REST APIs use a uniform interface
 
 ## REST APIs are designed around a ____. resources

 ## What is an identifer of a resource? Give an example.
 which is a URI that uniquely identifies that resource. 
 For example, the URI for a particular customer order might be:<br>
 `https://adventure-works.com/orders/1`
 ## What are the most common HTTP verbs?
uniform interface includes using standard HTTP verbs to perform operations on resources. 
The most common operations are GET, POST, PUT, PATCH, and DELETE.
 
 ## What should the URIs be based on?
 resource URIs should be based on nouns (the resource) 
and not verbs (the operations on the resource).

## Give an example of a good URI.
`https://adventure-works.com/orders`

## What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
avoid "chatty" web APIs that expose a large number of small resources. 

## What status code does a successful GET request return?
A successful GET method typically returns HTTP status code 200 (OK).

## What status code does an unsuccessful GET request return?
If the resource cannot be found, the method should return 404 (Not Found).

## What status code does a successful POST request return?
it returns HTTP status code 201 (Created). 
The URI of the new resource is included in the Location header of the response.

## What status code does a successful DELETE request return?
If the delete operation is successful,
the web server should respond with HTTP status code 204 (No Content), 
indicating that the process has been successfully handled
