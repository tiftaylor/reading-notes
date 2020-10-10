# Class 03 \| Data Modeling & NoSQL
Video: [SQL vs NoSQL](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)     
Article: [NoSQL vs SQL](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)  
Article: [NoSQL Modeling Techniques](https://highlyscalable.wordpress.com/2012/03/01/nosql-data-modeling-techniques/)   


## Review Tidbits

Name 3 advantages to Test Driven Development 
  - When you write tests first (per tradition), it helps you better understand how you'll write your function and will always fail until you've written your function correctly
  - Once a test is written, it can be reused over and over to ensure something from the past doesn't break as you continue to add new things to the code base
  - Writing a test first with your teammates can help everyone agree on what the function is supposed to do, up front.

In what case would you need to use beforeEach() or afterEach() in a test suite?
  - beforeEach and afterEach are ran before and after each test case and are used when you want to repeat a setup for many tests.

What is one downside of Test Driven Development
  - It's expensive. By that I mean, it takes a lot more man power hours and effort to create which is slow and time consuming.

What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?
  - I think it's just that ES6 classes help you do the same thing but in potentially less lines of code and lines of code that are easier to read as a developer than the traditional consturot/prototype way.

Name a use case for a static method
  - When you don't want the definition of the method to be changed or overridden (stay static).

Write an example of a Higher Order function and describe the use case it solves
  - Use case: when you want to have abstract control over actions (not just values) of past, present or future functions
  ```
    function greaterThan(n) {
      return m => m > n;
    }
    let greaterThan10 = greaterThan(10);
    console.log(greaterThan10(11));
    // → true
  ```
  - Example function borrowed from [Eloquent JavaScript](https://eloquentjavascript.net/05_higher_order.html)



**Document the following Vocabulary Terms**  
Term | Defition  
--|--  
functional programming | A style of programming that strictly uses math as its equation style and uses data that doesn't change (stateless?) and uses a declarative model and focuses on "what" you are doing and renders no side effects. 
pure function | there is no variation for it's variable which remains static. No input aspects from a device.
higher-order function | Kind of like a "father" function, it takes one or more functions as an argument and also returns a function (for my father analogy: is a human, takes another human and returns a new human)
immutable state | data that doesn't change
object | Basically, some data. It lives in `{}` in JS and can consist of anything, like variables, key/value pairs, functions, data structures, etc.
object-oriented programming (OOP) | Can use data that changes (mutable) and is considered an imperative model and focuses on "how" you are doing something. The methods used can cause side effects (unlike functional programming) and uses the "loop" concept for iteration. 
class | It's like a template for creating objects that provides inital states and behavior.
prototype | an objects private property that is a link to another object
super | Super keyword is used when referring to a class parent object
inheritance | When "something" is passed down to it's children code blocks/functions that impacts them / they are using from it's parent even though it isn't implicitly written in their block.
constructor | Similar to `class`, a template to use for making instances of an object.
instance | One specific creation of an object that was built from calling a `new` constructor and providing it paramaters
context | Simply put, the place within the scope of code of where you're currently working
this | a keyword in JS that is based on context of it's scope
Test Driven Development (TDD) | "Test-driven development (TDD) is a software development process that relies on the repetition of a very short development cycle: requirements are turned into very specific test cases, then the code is improved so that the tests pass." [Wikipedia](https://en.wikipedia.org/wiki/Test-driven_development)
Jest | "Jest is a delightful JavaScript Testing Framework with a focus on simplicity. It works with projects using: Babel, TypeScript, Node, React, Angular, Vue and more!" [jestjs.io](https://jestjs.io/)
Continuous Integration (CI) | "a development practice where developers integrate code into a shared repository frequently, preferably several times a day. Each integration can then be verified by an automated build and automated tests." [Codeship](https://codeship.com/continuous-integration-essentials#:~:text=Continuous%20Integration%20(CI)%20is%20a,automated%20build%20and%20automated%20tests.)
unit test | "typically automated tests written and run by software developers to ensure that a section of an application (known as the "unit") meets its design and behaves as intended. In procedural programming, a unit could be an entire module, but it is more commonly an individual function or procedure." [Wikipedia](https://en.wikipedia.org/wiki/Unit_testing#:~:text=Unit%20tests%20are%20typically%20automated,an%20individual%20function%20or%20procedure.)


## Upcoming Lecture

Which 3 things had you heard about previously and now have better clarity on?
  1) SQL is a language to make queries, not a database (good reminder!)
  2) SQL data structure is relationtional (has tables and clear schemas and records adhere to the schemas and data is normalized)
  3) MongoDB, I have seen this but didn't know it's connection to the NoSQL concept. It is database with collections of documents / not relational

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  1) Scaling? Horizontal vs. Vertical - what examples of needing to scale? And how does the direction of scaling impact needs? 
  2) I feel like my brain is missing context for when, how, why I need to think about all these data modeling techniques. 
  3) Just overall dumbing down of this entire topic into bite size baby steps of a real world example of why this topic matters to me.

What are you most excited about trying to implement or see how it works?
   - Inverted search aggregates


[Back to Home](README.md)