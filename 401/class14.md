# Class 14 \| Access Control ACL
Article: [RBAC Tutorial](https://www.youtube.com/watch?v=C4NP8Eon3cA)       
Article: [5 Steps to RBAC](https://www.csoonline.com/article/3060780/security/5-steps-to-simple-role-based-access-control.html)    
Article: [wiki - RBAC](https://en.wikipedia.org/wiki/Role-based_access_control)     


## Review Tidbits

When is Basic Authorization used vs. Bearer Authorization?
  - Bearer is token based, basic is not

What does the JSON Web Token package do?
  - creates and validates json web tokens

What considerations should we make when creating and storing a SECRET?
  - keep them hidden. Becareful what service you use to share the information with coworkers, don't check them into a code base (like use .env and have .gitignore that file), and because they aren't being logged on the console ever in errors or on purpose.

**Document the following Vocabulary Terms**  
Term | Defition  
--|--  
encryption | encoding info so unauthroized ppl can't read it - only servers @ "that" site can read it
token | a strong of characters that enables you to access things on an api
bearer | someone who has the token, you bear the token...
secret | something you don't want other ppl to know, like decryption key
JSON Web Token | standard for creating data with encryption whos payload is json format with identity info(signatures)


## Upcoming Lecture

Which 3 things had you heard about previously and now have better clarity on?
  - access control in general I was clear on, but it's great to see how this concept translates to tech roles
  - there are different access control system levels, like role vs attribute based

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  - How does this apply to what we'll be learning later this week 
  - What's the best practice on how and when to combine authoritzation with access system levels

What are you most excited about trying to implement or see how it works?
   - to understand better this access world we're playing with 


[Back to Home](README.md)