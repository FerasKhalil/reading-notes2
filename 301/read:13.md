# Read: Class 13 CRUD

### Status Codes Based On REST Methods

- 100’s = These are informational status codes; they usually tell the client that the header part of the request has been 
received and the server will try to comply with a transmission demand of the client. Like using a different protocol or 
telling the client that its request will fail before they start sending the body.


- 200’s = These are the success codes. They tell the client that its request was accepted. In case of asynchronous processing 
of a request (202), this doesn’t mean the request was successfully processed only that it met all validation requirements at
the time of sending.


- 300’s = These are redirection codes. They tell the client that the resource they are requesting isn’t available at the expected 
location anymore. This can have multiple reasons, be temporary or permanent, but the client has to issue a request to the new location.


- 400’s = These are the client error codes. They are all about invalid requests a client sent to a server. There are several causes to this,
 timeouts, wrong URI, missing authentication, etc. A client is sending incorrect input and should confirm the input parameters are correct
 before retrying the request.


- 500’s = These are the server error codes. Often they indicate problems with overwhelmed servers or unreachable servers behind proxies, but 
	- sometimes they can be directly related to client requests that trigger error exceptions on the server. These errors can be temporary or permanent.
 	Usually it’s best for the client to retry the same request.

- all form(https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

1. What is a status code 202?
	- Often used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime 
	  in the future. The response body should include an URL to the finished resource with some information about when it will be available, or an URL 
	 to some monitoring endpoint that tells the client when the resource is available.

2. What is a status code 308?
	- This tells the client to use another URL to access the resource and not use the current URL anymore. It’s helpful when we have multiple 
   	  endpoints for one resource, but don’t want to implement reading from all of them.

3. What code would you use if an update didn’t return data to a client?
	- 204 No Content.
		
4. What code would you use if a resource used to exist but no longer does?
	- PATCH.

5. What is the ‘Forbidden’ status code?
	- 403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.
	  from (https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/) .




6. Why do we need to pull our MongoDB database string out of our server and put it into our .env?
	- to connect our PORT.



7. What is middleware?
	- software which lies between an operating system and the applications running on it.
	- from (https://www.google.com/search?q=What+is+middleware%3F&oq=What+is+middleware%3F&aqs=chrome..69i57j0l9.434j0j7&sourceid=chrome&ie=UTF-8)


8. What does app.use(express.json()) do?
	- it calls json which is a method that is built inside the express, it converts the objects to arrays or strings 



## Things I want to know more about
all of it


