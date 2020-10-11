# Class 04 \| Advanced Mongo/Mongoose
Article: [The Repo Design Pattern](https://cubettech.com/resources/blog/introduction-to-repository-design-pattern/)       
Article: [In Memory Database Testing](https://dev.to/paulasantamaria/testing-node-js-mongoose-with-an-in-memory-database-32np)    
Article: [Mongo Memory Server](https://www.npmjs.com/package/mongodb-memory-server)     


## Review Tidbits

Why would a developer choose to make data models?
  - I assuemd a data model is required, so having to understand why we would chose to have one doesn't seem like a luxury a dev has, since they're necessary. But, I guess in essence, you make one to try and make your query life easier.

What purpose do CRUD operations serve?
  - It allows us to create, read, update, delete data to manipulate the front end of an application based on the users needs

What kind of database is Postgres? What kind of database is MongoDB?
  - Postgres is a SQL database that relies on sepcific schemas for a relational database quereies
  - MongoDB is a NoSQL database that isn't relational and all data is stored in documents in collections

What is Mongoose and why do we need it?
  - We use Mongoose to create classes (or models) for "mapping" from business logic to data structure. We need it to help keep queries centralized, and reduces dupicate code.

**Document the following Vocabulary Terms**  
Term | Defition  
--|--  
database | A structure that stores organized information, usually in the form of tables with fields
data model | A model taht organizes data and specifies how they relate to one another and to the real-world properties
CRUD | Acronym for SQL commands to Create, Read, Update, Delete
schema | the specific structure of a database (like identifying the column headings)
sanitize | This is when you completely delete some data and replace it with your new definition of data. The old or original data is no longer stored in memory after it's been sanitized 
Structured Query Language (SQL) | A language used to make queries against a relational database (BigTable style)
Non SQL (NoSQL) | A program used to make queries from data that isn't stored in a clear schema relational way
MongoDB | "MongoDB is a general purpose, document-based, distributed database built for modern application developers and for the cloud era." [mongodb.com](https://www.mongodb.com/) 
Mongoose | "Mongoose provides a straight-forward, schema-based solution to model your application data." It claims to be **mongodb** object modeling for **node.js** [mongoosejs](https://mongoosejs.com/) 
record | Like a specific row or object that contains values relating to it's keys (or fields) 
document | Tehcnically *document* is a model type for a nonrelational database. Works well with things like catalogs or user profiles 
Object Relation Mapping (ORM) | "Object-relational mapping in computer science is a programming technique for converting data between incompatible type systems using object-oriented programming languages. This creates, in effect, a "virtual object database" that can be used from within the programming language" [Wikipedia](https://en.wikipedia.org/wiki/Object%E2%80%93relational_mapping) 


## Upcoming Lecture

Which 3 things had you heard about previously and now have better clarity on?
  1) I had heard the word "system design" - is that the same thing as "software design patterns"?
  2) I had not heard about repository patterns but now I have, so naturally, better clarity :)
  3) I've heard of mongoDB, I maybe have better clarity on what it is, in that it's a sibling of postgres, and just another way to create and maintain

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  1) Understanding the difference between the data mapper vs. query object
  2) What does this look like in practice
  3) Just feeling a little overwhelmed and confused on the point of using mongoose (with?) mongoDB

What are you most excited about trying to implement or see how it works?
   - Looking forward to attempting to try MongoDB and see how similar or disimlar it is to postgres


[Back to Home](README.md)