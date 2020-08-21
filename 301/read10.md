# Read:10 \| The Call Stack
MDN: [The Call Stack Defined](https://developer.mozilla.org/en-US/docs/Glossary/Call_stack)   
Article: [Understanding the JS Call Stack](https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4) | Article: [JavaScript Error Messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

## Notes from [The Call Stack Defined](https://developer.mozilla.org/en-US/docs/Glossary/Call_stack)

> MDN defines "call stack" as:   
> A call stack is a mechanism for an interpreter to keep track of its place in a script that calls 
> multiple functions -- what function is currently being run, and what functions are called from 
> within that function, etc. 

- When a function is called in a script, the interpreter adds it to the call stack and starts carrying out the function.
- If a function is called by that original function, that is added to the call stack but further up.
- When a function is finished, it is removed from the stack and the interpreter resumes execution where it left off.
- "Stack overflow" is when the stack takes up more space than it had assigned to it.

  <image src="../images/read10-1.png" style="width: 300px">

- The call stack in the above image will look like this:
  - `sayHi`
  - `greeding`

- **Summary**: The call stack starts empty. When a function is called, it is automatically added to the call stack. When the function has executed, it is removed from the call stack, leaving the stack empty again.


## Notes from [Understanding the JS Call Stack](https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4)

- The call stack gives clarity to function hierarchy and execution order in the JS engine.
- It operates under the LIFO principle. The article describes LIFO as the following:

  > LIFO: When we say that the call stack, operates by the data structure principle of 
  > Last In, First Out, it means that the last function that gets pushed into the stack 
  > is the first to be popped out when the function returns.

- A function, its parameters, and its variables that are pushed into the call stack form a **stack frame** (memory location in the stack).
- Stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point.
- Call stack is single-threaded.
- Code execution is synchronous.


## Notes from [JavaScript Error Messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

- Types of error messages are:
  - Reference errors: tried to use a variable that is not yet declared. A simple fix is declaring the variables before any declaration is made. For example:
    ```js
    let foo;
    foo = 'Hello';
    ```
  - Syntax errors: come from misplaced quotes, semi-colons, parentheses, etc.
  - Range errors: when an object being manipulated that has length is given an invalid length (like negative).
  - Type errors: show up when types are incompatible (numbers, strings, etc).
- The easiest way to debug your JS is `console.log`
- You can use the Chrome Developer Tools using `cmd+o`. To choose a file to debug, click the line and refresh the page.
- You can also create a breakpoint with a `debugger` statement where you want to break.

  <image src="../images/read10-2.png" style="width: 300px">

- The call stack is given by the **red** part of an error message. The article explains how to use the debugger to analyze the call stack:

> Paired with breakpoints it is easier to create a code execution in scenarios 
> like this by taking into account the call stack which is available, for example, 
> in chrome developer tools “sources” tab.

- Naming functions makes the call stack easier to navigate.
- `console.trace()` prints out the current call stack trace.
- You can handle errors by using `try` and `catch`. For example:

  ```js
  (function testing(){
    function add(a, b) {
      try {
        var result = a + b
        return result.split('')
      } catch (error) {
        console.error('add went wrong ->', error)
        return [] // default value
      }
    }
    var stringResult = add("1", "2")
    var numberResult = add(1, 2)
  })()
  ```

- Because JS is not compiled, your errors happen at runtime. That means you can only see what's wrong after it is running.
- You can use tools like quokka, eslint, and TypeScript to detect errors faster.






[Back to Home](README.md)