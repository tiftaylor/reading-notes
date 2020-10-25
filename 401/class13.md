# Class 13 \| Bearer Authorization
Article: [JWTs Explained](https://www.youtube.com/watch?v=926mknSW9Lo)       
Article: [Intro to JWT](https://jwt.io/introduction/)    
Article: [Are JWTs Secure](https://stackoverflow.com/questions/27301557/if-you-can-decode-jwt-how-are-they-secure)     


## Review Tidbits

Write the following steps in the correct order:
  6 - Receive access token
  3 - Redirect to a third party authentication endpoint
  1 - Register your application to get a client_id and client_secret
  7 - Make a request to a third-party API endpoint
  2 - Ask the client if they want to sign in via a third party
  4 - Receive authorization code
  5 - Make a request to the access token endpoint


What can you do with an authorization code?
  - Get an access token

What can you do with an access token?
  - access the third party API data

What’s a benefit of using OAuth instead of your own basic authentication?
  - Basic auth usually for the user on your own site, oAuth usually for accesshing third party / allows the user to delegate to you ability to access another sites data with their "badge" (identity)


**Document the following Vocabulary Terms**  
Term | Defition  
--|--  
Client ID | public, used for longin URLs when signing up for Oauth serverice
Client Secret | this should be kept secret, you get this when creating a dev account with 3rd party oAuth service
Authentication Endpoint | redirect to 2rd party for user to login/accept it's ok fo ryour site to access
Access Token Endpoint | a url you post to in order to cash in the auth code
API Endpoint | a specific url route to get data from the api
Authorization Code | is a token that gets cashed in for a token, stored in url for giving access
Access Token | a string that should be stored as a secret to access third party api


## Upcoming Lecture

Which 3 things had you heard about previously and now have better clarity on?
  1) Signatures on JWT are what help prevent faud than just the payload encryption
  2) token vs. non-token authorization
  3) json web tokens - they contain a header/payload/signature

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  1) When do I not use JWT? 
  2) What is the best way to share secrets with teammates
  3) Bearer vs. OAuth and then when using both, OAuth that uses Bearer (like Yelp)

What are you most excited about trying to implement or see how it works?
   - Eager to see what it takes to make a user account feature on an app


[Back to Home](README.md)