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
  1) x
  2) y
  3) z

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  1) x
  2) y
  3) z

What are you most excited about trying to implement or see how it works?
   - xyz


[Back to Home](README.md)