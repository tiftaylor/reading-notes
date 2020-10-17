# Class 07 \| Express
Video: [Express Middleare Explained](https://www.youtube.com/watch?v=9HOem0amlyg)     
Article: [Using Express Middleware](https://expressjs.com/en/guide/using-middleware.html)  
Article: [Express Middleware](https://www.tutorialspoint.com/expressjs/expressjs_middleware.htm)   
Article: [Using Express Routing](https://expressjs.com/en/guide/routing.html)  


## Review Tidbits

What’s the difference between PUT and PATCH?
  - PUT gives a new version of the requested source and replaces original, whereas PATCH just gives instructions on how to modify the source

Provide links to 3 services or tools that allow you to “mock” an API for development like json-server
  - [JSON Placeholder](http://jsonplaceholder.typicode.com/)
  - [faker.js](https://github.com/Marak/faker.js)
  - [Mirage JS](https://www.valentinog.com/blog/fake/#mirage-js)

Compare and contrast Swagger and APIDoc.js Which HTTP status codes should be sent with each type of (un)successful API call?
  - 404 Not Found response for an operation that returns a resource by ID, or a 400 Bad Request response in case of invalid operation parameters.
  ```
  /users/{id}:
    get:
      summary: Gets a user by ID.
      response:
        200:
          description: OK
          schema:
            $ref: '#/definitions/User'
        401:
          $ref: '#/responses/Unauthorized'   
        404:
          $ref: '#/responses/NotFound'       
  ```
  - for APIDoc.js: `@apiErrorExample {json} Error-Response:`

Compare and contrast SOAP and ReST
  - ReST is newer than SOAP and aims to basically do things better that SOAP wasn't made to encounter originally and makes accessing web services simpler. Both provide a set of rules in an architecture which is helpful. Choosing one becomes more obvious based on the language you're programming in.

**Document the following Vocabulary Terms**  
Term | Defition  
--|--  
SOAP |  "Simple Object Access Protocol" /  invented by MS, been around a while. XML msging service
ReST Verbs |  GET (obtain data), POST (send new data), PUT (modify data), DELETE (remove data)
CRUD Verbs |  CREATE, READ, UPDATE, DELETE
Swagger |  Swagger is in essence an Interface Description Language for describing RESTful APIs expressed using JSON. Swagger is used together with a set of open-source software tools to design, build, document, and use RESTful web services. Swagger includes automated documentation, code generation, and test-case generation [resource](https://en.wikipedia.org/wiki/Swagger_(software))


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