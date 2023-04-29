# Reading notes for class 8

## API Design Best Practices

**What does REST stand for?**
Representational State Transfer.

**REST APIs are designed around a ____.**
Resource (any kind of object, data, or service that can be accessed by the client).

**What is an identifier of a resource? Give an example.**
A URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:

HTTP
://adventure-works.com/orders/1

**What are the most common HTTP verbs?**
GET, POST, PUT, PATCH, and DELETE.

**What should the URIs be based on?**
Nouns (the resource).

**Give an example of a good URI.**
A good URI will take in
-Stability over time
-Short
-Give the user an idea what is linked
-Easy to type
-Easy to guess (relevant only for a few links like "/jobs")
-Search engine friendly
-URI schema should be consistent over the whole site
-URI schema should allow future extensions

**What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?**
A chatty web API means that theres a lot of requests (or a bigger load) which overworks the API. This is a bad thing.

**What status code does a successful GET request return?**
200 (OK).

**What status code does an unsuccessful GET request return?**
404 (not found) if the resource can't be found. 204 (No content) is the request was successful but there is no response body included in the HTTP response.

**What status code does a successful POST request return?**
201(Created), or 200(OK).

**What status code does a successful DELETE request return?**
204(No content).

## Things I want to know more about

-Status codes and what they mean right away, but as I get more familiar with them I know that will come.
