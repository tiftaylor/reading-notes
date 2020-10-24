# Class 12 \| OAuth
Article: [What is OAuth Really All About](https://www.youtube.com/watch?v=t4-416mg6iU)       
Article: [OAuth2 Simplified](https://aaronparecki.com/oauth-2-simplified/)    
Article: [Build a Node API with OAuth](https://developer.okta.com/blog/2018/08/21/build-secure-rest-api-with-node)     


## Review Tidbits

Why is authentication important?
  - Enables user account funtionality on an application

Why should we be careful about storing a user’s password?
  - so the user account is protected from hacking/fraud/identity theft

What is the difference between hashing and encryption?
  - hasing is a one way translation / encryption is 2 way so the server can talk back to the client, etc

What is the difference between encryption and encoding?
  - well all encryption is encoded but not all encoded stuff is encrypted. Encrytpion has secrets and encoding doesn't always

What is a token used for?
  - If I have it, I'm allowed to do something - "ticket entry" to exclusive access

**Document the following Vocabulary Terms**  
Term | Defition  
--|--  
authentication | determing and validating the identity of the user
authorization | now that I have authenticated you, are you allowed to do this action?
encryption | encoding info so unauthroized ppl can't read it - only servers @ "that" site can read it
hashing | take some data, pass it through a hashing algo and get short data string in return that's unique
session | period of time where you are interacting with specific functionalities / has a clear start and end point
cookie | defines http headers, stores session information during the session, browsers own them, server can send new definitions to cookies while in session, they are scoped
token | a string that is used as input for acccessing secret things - it doesn't expire when used so is reusable and sharable
Basic Auth | 
encoding | code is in one format and is converted to another format for other systems to read
secret | something you don't want other ppl to know, like decryption key
cryptography | practice of techniques for secure communication 


## Upcoming Lecture

Which 3 things had you heard about previously and now have better clarity on?
  1) cookies - i'm slowly starting to understand what they are used for now
  2) token - i knew this, but good to have it confirmed
  3) authentication vs. authorization

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  1) 
  2) y
  3) z

What are you most excited about trying to implement or see how it works?
   - xyz


[Back to Home](README.md)