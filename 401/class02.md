# Class 02 \| Classes, Inheritance, Functional Programming
Video: [TDD in JS](http://www.letscodejavascript.com/)      
Video: [JavaScript Context Tutorial](https://www.youtube.com/watch?v=fjJoX9F_F5g)  
Article: [MDN Inheritance](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain)   
Article: [MDN this](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this)   
Article: [MDN - ES6 Classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)    


## Review Tidbits

Why would you want to run JavaScript code outside of a browser?
  - When you want to run a program that uses JS as it's backend language for programming continuity; when you want your whole stack to be in JS

What is the difference between a module and a package?
  - Nothing in the grand scheme. The word is interchangable. They are both things you can download or use with a CDN link to use their methods in your JS files. If you want to get picky, some say a **module** is a single file for use, whereas the **package** is several files and had a package.json with it

What does the node package manager do?
  - It's a command you can use in the terminal `npm install xyz` and it allows you to install, delete, update, create, etc packages. 

Provide code snippets showing 3 different ways to export a function from a node module
  - `module.exports.tea = tea;`
  - `module.exports = {Cat: Cat}`
  - `exports.foo = 'foo';`

**Document the following Vocabulary Terms**  
Term | Defition  
--|--  
ecosystem |  In the context of software analysis, the term software ecosystem is defined by Lungu as “a collection of software projects, which are developed and co-evolve in the same environment”. The environment can be organizational (a company), social (an open-source community), or technical (the Ruby ecosystem). [Software Ecosystem](https://en.wikipedia.org/wiki/Software_ecosystem#:~:text=In%20the%20context%20of%20software,technical%20(the%20Ruby%20ecosystem).)
Node.js |  An event-driven, non-block i/o JavaScript runtime (basically translates the frontend language JS into a usable back-end version of JS to work with servers and databases)
V8 Engine |  V8 is Google's open source high-performance JavaScript and WebAssembly engine, written in C++. It is used in Chrome and in Node. js, among others. It implements ECMAScript and WebAssembly, and runs on Windows 7 or later, macOS 10.12+, and Linux systems that use x64, IA-32, ARM, or MIPS processors. [v8.dev](https://v8.dev/)
module |  Also known as "package". JS files that contain reusable methods you can use in your project  BUT usually a single file not the full package with several
package |  Also known as "module". JS files that contain reusable methods you can use in your project OR it is a collection of modules that uses a package.json file
node package manager (npm) |  A website/registry that hosts open source packages for JavaScript. You can find or create packages through npm  
server |  A server is a computer or system that provides resources, data, services, or programs to other computers, known as clients, over a network. In theory, whenever computers share resources with client machines they are considered servers
environment |  An environment is the context in which code is executing. This includes all code executables and variables available to the code being executed. You can think of an environment as a unique machine executing code. Each machine is a different environment. [Linden Melvin](https://qr.ae/pNkqws)
interpreter |  In computer science, an interpreter is a computer program that directly executes instructions written in a programming or scripting language, without requiring them previously to have been compiled into a machine language program. [Wikipedia](https://en.wikipedia.org/wiki/Interpreter_(computing))
compiler |  A compiler is a special program that processes statements written in a particular programming language and turns them into machine language or "code" that a computer's processor uses. [tech target](https://whatis.techtarget.com/definition/compiler)


## Upcoming Lecture

Which 3 things had you heard about previously and now have better clarity on?
  1) ES6 Classes
  2) Inheritence
  3) Context

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  1) Test driven development - no idea anything about this yet
  2) Hoisting as classes
  3) object oriented design

What are you most excited about trying to implement or see how it works?
   - classes


[Back to Home](README.md)