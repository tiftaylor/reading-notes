# Class 09 \| API Server
Article: [Express Router.param() middleware](https://expressjs.com/en/4x/api.html#router.param)     
Article: [Mongoose Middleware](https://mongoosejs.com/docs/middleware.html)  
Article: [Mongoose sub-documents](https://mongoosejs.com/docs/subdocs.html)   
Article: [Mongoose Virtual Joins](https://mongoosejs.com/docs/populate.html#populate-virtuals)  


## Review Tidbits

How does route prefixing work with an external routing module?
  - Set of routes that are added to your app under a shared path

When routing, what’s the difference between app.get('/data/:id') and app.get('/data/:name')?
  - They are different names in the handler function that refer to the req.params

Explain how Express handles routing conflicts?
  - The first match takes priority

What are the ways that a browser can send “data” or request variables to an HTTP server
  - req.body // http verbs for it are POST, PATCH, PUT, also can be headers and GET but don't use get since that puts data in the url which isn't private


**Document the following Vocabulary Terms**  
Term | Defition  
--|--  
Routing |  URIs mapped to handlers that communicate stuff
Route Prefixing |  The default path used in front of /params
Request “Body” |  contains data sent back to client, like in the form of JSON
Request “Query” |  gives the query param values
Request “Params” |  defined by URL for what data you want the server to look at



## Upcoming Lecture

Which 3 things had you heard about previously and now have better clarity on?
  1) Slowly wraping my head around router.param / router lvl stuff
  2) router.route - cool ok so I kinda get the instance aspect where the HTTP methods will only apply to that instance of that route url
  3) Slowly understanding the concept of middleware, didn't realize Mongoose itself ad 4 different types! Bigger world than I thought

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  1) Still not clear on express.static() - where/what/when/how/why
  2) I need more examples and human explanation of when/where/why for next()
  3) Break down the concept and definitions and use of hooks (vs. no hooks?)

What are you most excited about trying to implement or see how it works?
   - I'm not sure i'm excited about any of this haha, backend stuff is pretty hard for me. So just looking forward to continuing to attempt to implement anything


[Back to Home](README.md)