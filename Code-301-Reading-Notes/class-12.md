# class-12

## In your own words, describe what each group of status code represents:
* 100’s =These are informational status codes; they usually tell the client that
 the header part of the request has been received and the server will try to comply with a transmission demand of the client.
* 200’s = These are the success codes. They tell the client that its request was accepted. In case of asynchronous processing of a request (202),
* 300’s = These are redirection codes. They tell the client that the resource they are requesting isn’t available at the expected location anymore.
* 400’s = These are the client error codes. They are all about invalid requests a client sent to a server. There are several causes to this,
* 500’s = These are the server error codes. Often they indicate problems with overwhelmed servers or unreachable servers behind proxies,

## What is a status code 202?
Accepted - If the update is done asynchronous, this code can be used.
It should include an URL to access the updated resource or
an URL to check if the update has been succeeded. <br> 

 Often used for asynchronous processing. 
 This code tells the client that the request was valid,
 but its processing will finish sometime in the future. 
 
 ## What is a status code 308?
 Permanent Redirect - This tells the client to use
 another URL to access the resource and not use the current URL anymore.<br>
 
 This would be the right code if we know that a resource 
 has moved to a different URL and we can tell the client about it.
 
 
 ## What code would you use if an update didn’t return data to a client?
 
 204 No Content - A proper code for updates that don’t return data to the client, 
 for example when just saving a currently edited document.

## What code would you use if a resource used to exist but no longer does?
406 Not Acceptable - The URL exists, but the backend can’t send a representation the client will accept. So for that specific client, the URL behaves like a 404
, but they now know that they need to update the client.

## What is the ‘Forbidden’ status code?
403 Forbidden - The client has authorized or doesn’t need to authorize itself, 
but still has no permissions to access the resource.

## Why do we need to pull our MongoDB database string out of our server and put it into our .env?
* Create an Atlas Account and Cluster
* Set Up Connectivity to Atlas

## What is middleware?
Middleware is software that provides common services and capabilities to applications outside of what’s offered by the operating system. 

## What does app.use(express.json()) do?
The express.json() function is a built-in middleware function in Express. It parses incoming requests with JSON payloads and is based on body-parser.

## What is the difference beween PUT and PATCH?
PUT HTTP Request: PUT is a method of modifying resources where the client sends data that updates the entire resource. PUT is similar to POST in that it can create resources, 

<br>
PATCH HTTP Request: Unlike PUT Request, PATCH does partial update e.g. Fields that need to be updated by the client, only that field is updated without modifying the other field.



