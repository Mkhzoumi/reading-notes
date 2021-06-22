# CRUD




## In your own words, describe what each group of status code represents:
+ ## 100’s = These are informational status codes; they usually tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client. 
+ ## 200’s = These are the success codes. They tell the client that its request was accepted. 
+ ## 300’s = These are redirection codes. They tell the client that the resource they are requesting isn’t available at the expected location anymore.
+ ## 400’s = These are the client error codes. They are all about invalid requests a client sent to a server. 
+ ## 500’s = These are the server error codes. Often they indicate problems with overwhelmed servers or unreachable servers behind proxies, 
    
## What is a status code 202?
+ ## 202 Accepted - Often used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime in the future.

## What is a status code 308?
+ ## 08 Permanent Redirect - This is the right code if the resource will now be available at a new URL and the client should directly access it via the new URL in the future.



## Why do we need to pull our MongoDB database string out of our server and put it into our .env?
+ ## Because mongoDB strings inside the application and when we deploy the application we use something is not our localhost

## What is middleware?
+ ## it's code that run when the server get the request.

## What does app.use(express.json()) do?
+ ## to Let the server accept JSON as a body.

## What does the /:id mean in a route?
+ ## It's a parameter that we can access in request.

## What is the difference beween PUT and PATCH?
+ ## ues patch for update because we only need to update bases into the user passes.

## How do you make a defalut value in a schema? by using default and set the value that you want What does a 500 error status code mean?
+ ## means there is an error on the server.

## What is the difference between a status 200 and a status 201?
+ ## 201 is more specific, 200 means everything is successfull.








# [back](../README.md)