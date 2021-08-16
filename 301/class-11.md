# **Class 11**  

## **What is OAuth**  

>#### What is OAuth? 

>>Answer,  
>>>#OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization.  
>>>>Roger A. Grimes and Josh Fruhlinger

>#### Give an example of what using OAuth would look like.

>>Answer,  
>>>let's say i go to a new website X and it requires a log in,  
Because this is my first time when i go to sign up i'm given an option to use my google account,  
This is OAuth because my identity was recognize without me signing up a new account because i gave it permission to use my google credentials, 

>#### How does OAuth work? What are the steps that it takes to authenticate the user?  

>>Answer,    
1. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
1. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
1. The first site gives this token and secret to the initiating user’s client software.
1. The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
1. If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
1. The user approves (or their software silently approves) a particular transaction type at the first website.
1. The user is given an approved access token (notice it’s no longer a request token).
1. The user gives the approved access token to the first website.
1. The first website gives the access token to the second website as proof of authentication on behalf of the user.
1. The second website lets the first website access their site on behalf of the user.
1. The second website lets the first website access their site on behalf of the user.


>#### What is OpenID?

>>Answer,  
>>>StackOverflow pithily put it: "OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans."

## **Authorization and Authentication flows** 

>#### What is the difference between authorization and authentication?

>>Answer,  
>>>In simple terms, authentication is the process of verifying who a user is, while authorization is the process of verifying what they have access to.  
>>>>Auth0 Docs

>#### What is Authorization Code Flow?

>>Answer,  
1. The user clicks Login within the regular web application.
1. Auth0's SDK redirects the user to the Auth0 Authorization Server (/authorize endpoint).
1. Your Auth0 Authorization Server redirects the user to the login and authorization prompt.
1. The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the regular web application.
1. Your Auth0 Authorization Server redirects the user back to the application with an authorization code, which is good for one use.
1. Auth0's SDK sends this code to the Auth0 Authorization Server (/oauth/token endpoint) along with the application's Client ID and Client Secret.
1. Your Auth0 Authorization Server verifies the code, Client ID, and Client Secret.
1.Your Auth0 Authorization Server responds with an ID Token and Access Token (and optionally, a Refresh Token).
1. Your application can use the Access Token to call an API to access information about the user.
1. The API responds with requested data.  
Auth0 Docs.


>#### What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

>>Answer,  
1. The user clicks Login within the application.
1. Auth0's SDK creates a cryptographically-random code_verifier and from this generates a code_challenge.
1. Auth0's SDK redirects the user to the Auth0 Authorization Server (/authorize endpoint) along with the code_challenge.
1. Your Auth0 Authorization Server redirects the user to the login and authorization prompt.
1. The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the application.
1. Your Auth0 Authorization Server stores the code_challenge and redirects the user back to the application with an authorization code, which is good for one use.
1. Auth0's SDK sends this code and the code_verifier (created in step 2) to the Auth0 Authorization Server (/oauth/token endpoint).
1. Your Auth0 Authorization Server verifies the code_challenge and code_verifier.
1. Your Auth0 Authorization Server responds with an ID Token and Access Token (and optionally, a Refresh Token).
1. Your application can use the Access Token to call an API to access information about the user.
1. The API responds with requested data.  
Auth0 Docs.

>#### What is Implicit Flow with Form Post?

>>Answer,  
1. The user clicks Login in the app.
1. Auth0's SDK redirects the user to the Auth0 Authorization Server (/authorize endpoint) passing along a response_type parameter of id_token that indicates the type of requested credential. It also passes along a response_mode parameter of form_post to ensure security.
1. Your Auth0 Authorization Server redirects the user to the login and authorization prompt.
1. The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the app.
1. Your Auth0 Authorization Server redirects the user back to the app with an ID Token.  
Auth0 Docs.


>#### What is Client Credentials Flow?

>>Answer,  
1. Your app authenticates with the Auth0 Authorization Server using its Client ID and Client Secret (/oauth/token endpoint).
1. Your Auth0 Authorization Server validates the Client ID and Client Secret.
1. Your Auth0 Authorization Server responds with an Access Token.
1. Your application can use the Access Token to call an API on behalf of itself.
1. The API responds with requested data.  
Auth0 Docs.

>#### What is Device Authorization Flow?

>>Answer,  
1. The user starts the app on the device.
1. The device app requests authorization from the Auth0 Authorization Server using its Client ID (/oauth/device/code endpoint).
1. The Auth0 Authorization Server responds with a device_code, user_code, verification_uri, verification_uri_complete expires_in (lifetime in seconds for device_code and user_code), and polling interval. 
1. The device app asks the user to activate using their computer or smartphone
1. The device app begins polling your Auth0 Authorization Server for an Access Token (/oauth/token endpoint) using the time period specified by interval and counting from receipt of the last polling request's response. The device app continues polling until either the user completes the browser flow path or the user code expires.
1. When the user successfully completes the browser flow path, your Auth0 Authorization Server responds with an Access Token (and optionally, a Refresh Token). The device app should now forget its device_code because it will expire.
1. Your device app can use the Access Token to call an API to access information about the user. 
1. The API responds with requested data.  
Auth0 Docs.

>#### What is Resource Owner Password Flow?

>>Answer,  
1. The user clicks Login within the application and enters their credentials.
1. Your application forwards the user's credentials to your Auth0 Authorization Server (/oauth/token endpoint).
1. Your Auth0 Authorization Server validates the credentials.
1. Your Auth0 Authorization Server responds with an Access Token (and optionally, a Refresh Token).
1. Your application can use the Access Token to call an API to access information about the user.
1. The API responds with requested data.  
Auth0 Docs.

