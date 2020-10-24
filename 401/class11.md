# Class 11 \| Authentication
Article: [Securing Passwords](https://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html)       
Article: [Basic Auth](https://en.wikipedia.org/wiki/Basic_access_authentication)    
Article: [Intro to JWT](https://jwt.io/introduction/)     
Article: [OWASP Auth Cheatsheet](https://www.owasp.org/index.php/Authentication_Cheat_Sheet)    
Article: [Bcrypt Docs](https://www.npmjs.com/package/bcrypt)    


## Review Tidbits

Explain what a “Singleton” is (in Computer Science terms)
  - Basically this is a design pattern where only 1 insertion of an instance happens

Explain how the Singleton pattern can be used with Node modules, specifically with classes
  - When a new instance is only created once, like during the module.exports stage, and if the instance needs to be used again, the fn's just use a copy of the initial instantion

If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?
  - I would use a doubly linked list approach because while things append (like .use()), being able to iterate from both directions would be ideal


**Document the following Vocabulary Terms**  
Term | Defition  
--|--  
Router Middleware | a sub middleware that sidetracks a command from app level and houses it's own middleware functions on specific routes at the router level  
Dynamic Module Loading | basically wrapping your require statments in a conditional like `if(x){req(this file)}`
Singleton Pattern | Please see answers to the first two questions up above  
CRUD -> REST Method Matches | Create=POST, Read=GET, Update=PUT, Delete=DELETE
Mock Testing | using any fake data to run your tests in your test file. 


## Upcoming Lecture

Which 3 things had you heard about previously and now have better clarity on?
  1) OAuth, I now now the O stands for open
  2) HTTP headers - I guess I understand now they are associated with basic auth and are encoded
  3) Authentication vs. authorization

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  1) OAuth, not sure why more difficult if it's "open"
  2) Hashing algorithms. Are they always the same code? Doesn't that make famous ones vulnerable if you know the code? 
  3) how session and cookie relate

What are you most excited about trying to implement or see how it works?
   - using oAuth APIs so I can get interesting social media data


[Back to Home](README.md)