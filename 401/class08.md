# Class 08 \| Express Routing & Connected API
Article: [Using Express Routing](https://expressjs.com/en/guide/routing.html)     
Article: [Express Routing](https://scotch.io/tutorials/learn-to-use-the-new-router-in-expressjs-4)  


## Review Tidbits

Name 3 real world use cases where you’d want to change the request with custom middleware
  - when you want to identify the currently logged in user on a request
  - when you want to always set a custom header on the res object
  - when you need to run various validation code

True or false: The route handler is middleware?
  - True

In what ways can a middleware function end the process and send data to the browser?
  - by using res.send() or res.end()

At what point in the request lifecycle can you “inject” middleware?
  - I'm not sure I understand the question. Based on reading I feel like the entire request cycle involves middleware, as opposed to it being injected at some later point. You can't request without the middleware handling the request lifecycle in full for you.

What can cause express to error with “Request headers sent twice, cannot start a second response”
  - when more than one response is trying to be sent to the client, like if you forget to write code to have it exit the function

**Document the following Vocabulary Terms**  
Term | Defition  
--|--  
Middleware |   software that acts as a bridge between an operating system or database and applications, especially on a network. [resource](https://languages.oup.com/google-dictionary-en)
Request Object |  reps the HTTP request with properites - the object that asks the server for something
Response Object |  this is what reps the HTTP response and carries back the information to the client
Application Middleware|  is when you want the middleware affecting and talking to your entire application and talks to other applications
Routing Middleware |  just like app level except it is glued to a specific instance of express.router() method



## Upcoming Lecture

Which 3 things had you heard about previously and now have better clarity on?
  1) General routing of HTTP using express app level route methods
  2) Slowly understanding how route paths works...
  3) route handlers, basically the function that carries out the path's needed actions

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  1) Still want to talk more about when / why using router level
  2) Login routing ?
  3) still not sure about how to include regex in a route path(parameter?)

What are you most excited about trying to implement or see how it works?
   - the difference in app level and router level middleware


[Back to Home](README.md)