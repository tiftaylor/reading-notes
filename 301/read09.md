# Read:09 \| Functional Programming
Article: [Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa) | Article: [Refactoring JS for Readability](https://dev.to/healeycodes/refactoring-javascript-for-performance-and-readability-with-examples-1hec)  

## Notes from [Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

Functional programming is the computation of mathematical functions that works to avoid mutable data

### Pure functions

- Pure functions will give the same result if given the same arguments repeatedly and do not cause noticeable side effects.
- A function will be impure simply if a global object was not passed as a parameter to the function
- A function can be pure if it doesn't refer to an external declared object
- Here is an example of a function that is pure because it takes `pi` as a parameter instead of using `num`:
  ```js
  let num = 3.14;
  const calculateArea = (radius, pi) => radius * radius * pi;
  calculateArea(10, num); // returns 314.0
  ```
- Just like when trying to avoid using a global variable as a parameter when declaring a function, try to avoid reading external variables.
- The definition of a noticeable side-effect from above includes modifying a global object or a parameter that is passed by reference.
- Here is a **impure** counter function:
  
  <image src="../images/read9-1.png" style="width: 300px">

- Here is the same function, but **pure**:

  <image src="../images/read9-2.png" style="width: 300px">

- Typically, we would use a `for` loop for iteration but it makes the variables mutable (**this is not ideal**). Instead, let's use **recursion**!!!

- This is an example of writing a counter with **mutable variables** (not ideal):

  <image src="../images/read9-3.png" style="width: 400px">

- Use **recursion** to avoid mutability while iterating (this is better!):

  <image src="../images/read9-4.png" style="width: 400px">

### Misc stuff

- When you have **pure functions** + **immutable data** = **referential transparency**.
- **First-class entities** is what you call a function that is also treated as a value used as data.
  - The first-class function can be referred to by constants and variables
  - Pass it as a parameter to other functions
  - Return it as a result from other functions
- When functions have similar logic but different operators (like addition vs. subtraction), you can build a function that receives the operator function and uses it inside the other function:

  <image src="../images/read9-5.png" style="width: 400px">

- Higher-order functions take one or more functions as **arguments** or **return** a function as its result.
  - The `doubleOperator` function in the above screenshot is considered higher-order.
- `Array.filter` is a function that expects `true` or `false`. For example, if the callback expression is true, the filter function will include the element in the result.
- The below screenshots will show how to filter even numbers the bad (mutable) way, and then the good (immutable) way:
  
  <image src="../images/read9-6.png" style="width: 400px">

- Another example of if you want to filter a given array of integers and output the values that are less than a specified value `x` -- instead of a for loop in one function, use a pure **declarative** like the screenshot below:

  <image src="../images/read9-7.png" style="width: 400px">

- The `Array.map` method **transforms** a collection by applying a function to all of its elements and building a **new** collection from the **returned values**.

  <image src="../images/read9-8.png" style="width: 400px">

- Here is an example of a higher-order function using `map`:

  <image src="../images/read9-9.png" style="width: 400px">

- `reduce` receives a function and a collection and returns a value created by combining the items. For example, a way to get the total amount is to compose `map` and `reduce` as in the below **pure** example:
  - `getAmount` receives the product object and returns only the `amount` value and the `reduce` combines all items by adding up:

  <image src="../images/read9-10.png" style="width: 400px">

### Here is your ultimate goal when utilizing `filter`, `map`, and `reduce` with **pure functionality**:

- <image src="../images/read9-11.png" style="width: 400px">


## Notes from [Refactoring JS for Readability](https://dev.to/healeycodes/refactoring-javascript-for-performance-and-readability-with-examples-1hec)

- It is good to check your code for any possible refactoring before submitting a PR
- Below is an example from the article about some code they refactored to prevent possible issues: 
```js
// Unrefactored code

const friendlyWords = require('friendly-words');

function randomPredicate() {
  const choice = Math.floor(Math.random() * friendlyWords.predicates.length);
  return friendlyWords.predicates[choice];
}

function randomObject() {
  const choice = Math.floor(Math.random() * friendlyWords.objects.length);
  return friendlyWords.objects[choice];
}

async function createUser(email) {
  const user = { email: email };
  user.url = randomPredicate() + randomObject() + randomObject();
  await db.insert(user, 'Users')
  sendWelcomeEmail(user);
```
```js
// Refactored code

const friendlyWords = require('friendly-words');

const generateURL = user => {
  const pick = arr => arr[Math.floor(Math.random() * arr.length)];
  user.url = `${pick(friendlyWords.predicates)}-${pick(friendlyWords.objects)}` +
    `-${pick(friendlyWords.objects)}`; // This line would've been too long for linters!
};

async function createUser(email) {
  const user = { email: email };
  // The URL-creation algorithm isn't important to this function so let's abstract it away
  generateURL(user);
  await db.insert(user, 'Users')
  sendWelcomeEmail(user);
}
```
- The above example inlined a function called `pick` th accept an array and return a random choicethen used a template literaly to build a URL
- There are no absolutes for clean code, so it's case by case.
- Here are general tips: 
  - Return early from functions
  - Cache variables so functions can be read like sentences
  - Check for web APIs before implementing your own functionality




[Back to Home](README.md)