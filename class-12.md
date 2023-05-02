# Reading notes for class 12

## Status Codes Based On REST Methods

**In your own words, describe what each group of status code represents:**

100’s = Informational status codes. They tell you request has been received and the server will try to comply with a transmission demand of the client
200’s = Success status codes, meaning the request was accepted.
300’s = Redirection codes, meaning the resource they are requesting aren't available at the expected location anymore.
400’s = Error codes, all about invalid requests a client sent to a server. Causes such as timeouts, wrong URI, and missing authentication.
500’s = Server error codes. These are problems with overwhelmed servers or unreachable servers behind proxies, but sometimes they can be directly related to client requests that trigger error exceptions on the server

**What is a status code 202?**
Asynchronous processing of a request (202), doesn’t mean the request was successfully processed only that it met all validation requirements at the time of sending.

**What is a status code 308?**
Permanent Redirect - This tells the client to use another URL to access the resource and not use the current URL anymore. It’s helpful when we have multiple endpoints for one resource, but don’t want to implement reading from all of them.

**What code would you use if an update didn’t return data to a client?**
Code 204, No Content.

**What code would you use if a resource used to exist but no longer does?**
Code 410, Gone. This is similar to 404 but we know that the resource existed in the past, but it got deleted or somehow moved, and we don’t know where.

**What is the ‘Forbidden’ status code?**
Code 403, Forbidden. The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

## Build A REST API With Node.js, Express, & MongoDB - Quick - First 20 minutes

**Why do we need to pull our MongoDB database string out of our server and put it into our .env?**

**What is middleware?**
Middleware is a function that will have all the access for requesting an object, responding to an object, and moving to the next middleware function in the application request-response cycle.

**What does app.use(express.json()) do?**
It is a built-in middleware function in Express that parses incoming requests with JSON payloads and is based on body-parser. Returns middleware that only parses JSON and only looks at requests where the Content-Type header matches the type option.

**What does the /:id mean in a route?**
From our list of routes, /:id is the path that gets you to this function. The “:id” specifies that whatever you put into that position will be passed as the id in the params map.

**What is the difference between PUT and PATCH?**
PUT is a technique of altering resources when the client transmits data that revamps the whole resource. PATCH is a technique for transforming the resources when the client transmits partial data that will be updated without changing the whole data.

**How do you make a default value in a schema?**
{ type: String, default: '' }

**What does a 500 error status code mean?**
500 Internal Server Error server error response code indicates that the server encountered an unexpected condition that prevented it from fulfilling the request.

**What is the difference between a status 200 and a status 201?**
200: “Everything is OK.” This is the code that is delivered when a web page or resource acts exactly the way it's expected to. 201: “Created.” The server has fulfilled the browser's request, and as a result, has created a new resource.

## Things I want to know more about

I want to know more about the errors and be able to know off the top of my head. I also want to be able to understand the PUT and PATCH.
