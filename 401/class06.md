# Class 06 \| HTTP and REST
Article: [HTTP Basics](https://code.tutsplus.com/tutorials/http-the-protocol-every-web-developer-must-know-part-1--net-31177)     
Article: [What is ReST](https://restfulapi.net/)  
Video: [HTTP & Rest](https://www.youtube.com/watch?v=Q-BpqyOT3a8)   


## Review Tidbits

Define three related pieces of data in a possible application. An example for a store application might be Product, Category and Department. Describe the constraints and rules on each piece of data and how you would relate these pieces to each other. For example, each Product has a Category and belongs in a Department.
  - In a Messaging App example, three data pieces are User, Image and Message. Message is from a user and to a user. User has none or more other users on a friends list. Image and text are types of messages.

What is the advantage of an ORM, like Mongoose?
  - While there is a cost with using ORM, it seems to possibly make your life better as a dev by enabling a use of a higher level API with more intuitive methods and less code to write.

How does the repository pattern compare with an ORM?
  - Repositories deal with Domain/Business objects (from the app point of view), an ORM handles db objects. A business objects IS NOT a db object, first has behaviour, the second is a glorified DTO, it only holds data. ... You can also check this post about more details about the repository pattern. [resource](https://stackoverflow.com/questions/10155517/repository-pattern-vs-orm#:~:text=Repositories%20deal%20with%20Domain%2FBusiness,DTO%2C%20it%20only%20holds%20data.&text=You%20can%20also%20check%20this,details%20about%20the%20repository%20pattern.)

When making a repository/facade, what flexibility do you gain?
  - When you want to change data storage all you have to do is change code on the collection file

Name 3 cloud based NoSQL Databases
  - MongoDB Atlas, Microsoft Azure, Amazon DynamoDB


**Document the following Vocabulary Terms**  
Term | Defition  
--|--  
lifecycle | Stages data goes through from start to when archieved. 6 Stages: Generation, Maintence, Active use, Publication, Archieving, Purging
collections |  document based sotrage system that is considered non-relational
the “Repository” design pattern |  
mongoose middleware | please see the defention of ORM below because to me it's the same
Object Relation Mapping (ORM) |  An example is Mongoose, which is a library to help with CRUD logic between JS and a server technology like MongoDB


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


[Back to Home](/README.md)