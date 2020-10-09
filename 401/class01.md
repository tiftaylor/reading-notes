# Class 01 \| Node Ecosystem, TDD, CI/CD
Article: [NodeJS Introduction](https://www.w3schools.com/nodejs/nodejs_intro.asp)     
Article: [What is NodeJS](https://www.freecodecamp.org/news/what-exactly-is-node-js-ae36e97449f5/)  
Article: [What is npm](https://docs.npmjs.com/about-npm/index.html)    


## Review Tidbits

Describe (in plain English) what Array.map() does: 
  - array.map() is used when A) you want the output to return an array and B) when you want the iteration to happen to every element of the original array.

Describe (in plain English) what Array.reduce() does: 
  - A method that uses a callback function on each array element using it's current value in the array and usually an accumulator value, resulting a single output at the end of all iterations.

Provide code snippets showing how to use superagent() to fetch data from a URL and log the result
  - With normal Promise .then() syntax
  ```
    function getCharacters() {
      superagent.get(swapi)
      .then( data => {
        let mainObj = data.body;
        let key = mainObj.name;
        let value = mainObj.url;
        let newObj = {
          [key]: value
        };

        console.log(newObj);
      })
      .catch(err => console.error(err));
    }
  ```

  - Again with async / await syntax
  ```
    async function getCityData(city) {
      let results = await superagent.get('https://geocode.xyz/seattle?json=1');
      console.log(results.body.longt, results.body.latt);
    }
  ```

Explain promises as though you were mentoring a Code 301 level student: 
  - Promises are kind of like what you did with superagent.get().then() during your last 2 weeks of the course; so if not using superagent you would use something like `new Promise`. Ultimately, you're going to report back if youo did or did not resolve something, and depending on that outcome, you will `.then()` do something. 

Are all callback functions considered to be Asynchronous? Why or Why Not?
- Yes, callback functions are asynchronous because they are simply functions used as an argument in another function which performs work in the background until it is done.



## Upcoming Lecture

Which 3 things had you heard about previously and now have better clarity on?
  1) Node.js is a runtime environment
  2) non-blocking I/O
  3) npm has packages for front and back end

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  1) "It has hooks that allow you to write your own C++ code that you can make available to JavaScript" - from article [What is NodeJS](https://www.freecodecamp.org/news/what-exactly-is-node-js-ae36e97449f5/)
  2) Using the CLI
  3) Managing version changes

What are you most excited about trying to implement or see how it works?
   - My needs for npm are still too vague and I'm not really able to come up with an idea of what I'm excited to implement. I expect exceitment or being able to articulate a desire of something specific will come naturally as I learn more and more while in lecture.


[Back to Home](README.md)