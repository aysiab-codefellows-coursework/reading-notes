# Reading Assignment 07

### Review, Research & Discussion
> 1. The correct order:
 - register your application to get a client_id and client_secret
- ask the client if they want to sign in via a third party
- redirect to a third party authentication endpoint
- make a request to a third-party API endpoint
- recieve authorization code
- make a request to eh access token endpoint
- recieve access token

> 2. What can you do with an authorization code?
- An authorization code is techically a temporary code that the client side can exchange for an access token. 

> 3. What can you do with an access token?
- Access tokens can be used to provide secure authorization to the API information

> 4. What's a benefit of using OAuth instead of your own basic authentication?
-  OAuth protects the user's basic auth with an access token.

### Definitions
**Client ID:** a public identifier for application that is unique for every client the server handles 
**Client Secret:** a secret only known to the app and the authorization server 
**Authentication Endpoint:** the middleware to authenticate users 
**Access Token Endpoint:** the middleware 
**API Endpoint:** where (after authorization usually) a client can access certain data from the API
**Authorization Code:** temporary generate code that is used to exchange for an access token to access the application.
**Access Token:** the token that allows an application to access endpoints from the API