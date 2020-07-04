# Read:02 \| Basics of HTML, CSS & JS
Textbook: _Jon Duckett: HTML & CSS_ + JavaScript & jQuery  
*(HTML book: Chapters 2 + 10 \| JS book: Chapters 2 + 4)*

---
## HTML Text/Tags
---
- HTML uses tags (elements) as it's markup language to bring structural and semantic meaning to text on the web page
- Structural Markup: elements used to describe the structure of the page like headings and paragraphs 
  - Ex: a simple `<p>` tag to indicate the text between these tags is regular paragraph style text
- Semantic Markup: elements that provide extra information like when you want something emphasized 
  - Ex: `<strong>` styling around text within a structural markup tag

Example of HTML using a structural (`<h1>` & `<p>`) + semantic (`<strong>`) tags: 
```
<html>
  <head>
    <title>My Webpage</title>
  </head>
<body>
  <h1>Welcome to my page!</h1>
  <p>This page will show you <strong>awesome</strong> things</p>
</body>
</html>
```
---
## Intro to CSS
---
- CSS creates style rules for everything in the body tag
- You assign properties to html elements, ids, or classes
- Each css declaration needs to contain the property and its value
- The css sheet is linked in the html ```<head>``` tag using the `<link>` html element
- You can use `<style>` tag for inline CSS in the HTML document but it's not preferred
- CSS rules have specificity hierarchy and inheritance 
  - Video Tutorial: *[Learn CSS Specificity in 11 Minutes](https://youtu.be/CHyPGSpIhSs)* by Web Dev Simplified

---
## JavaScript Lingo
---
- **Statements**: are instructions and each one starts a new line; can be organized in code blocks and usually end with `;`
- **Comments**: Single line comments explaining the code near it is written with `//` before the text (multi-line uses `/* */`)
- **Variables**: declare them like this `var thing;`, assign them using `=` 
  - Ex: `thing = 3;`
- Variable Names can’t start with a number, cannot use - or . and use camelCase
- **Data Types**: Numeric data (0.75), String data (“Hello”), Boolean Data (true/false)

### JS Arrays
- **Arrays** can story a list of multiple values to a single variable (the data types in the array do not need to be the same but its best practice to keep same data type to an array)
  - Ex: `var myColorArray = [Red, White, Blue];`
- Each *item* in an array is assigned an **index** which is how the various values are accessed. Index always starts at **0**
  - Ex: Looking at `myColorArray` even though there are **3** values in the array, because the index starts at **0**, this will mean `Red` is at index `0`, `White` is index `1`, etc.
- To **access** or **change** the index you use the array `name[]` with a square bracket that will store the index
  - Ex: `var blue = myColorArray[2];`

### JS Expressions + Operators
- Expressions evaluate into a result with a single value
- Operators dictate what calculations should occur when a programmer uses an expression
- Types of Operators are: *Assignment* (=), *Arithmetic* (*), *String* (+), *Comparison* (>), and *Logical*(&&)

Example using operators:
```
var num1 = 5;
var num2 = 10;
var total = num1 * num2
// Note: the total will equal 50
```

### JS Decisions 
- Your JS code will ultimately be analyzing *Evaluations*, *Decisions* and *Loops* to determine when to run which code
- You can visualize a decision being made using a flow chat like this: 
![Decision Flow Chart]()
- Decisions come from evaluating expressions and executing conditional statements (like `if/then/else`)
- Comparison operators are heavily relyed in JS decision making:
  ##### Comparison & Logical Operators 
  - Here is a list of the comparison operators:   
    > `==` `===` `!=` `!==` `>` `<` `>=` `<=`
  - Comparison operator `==` and `===` differ only in that `===` won’t auto-convert the data type and is therefore the more secure one to use
  - With the Comparison not equal to something, it’s better to use !== to preserve the data type
  - Logical operators allow you to compare more than one Comparison operator
  - **Logical Operators** are: 
    > `&&` (and), `||` (or), `!` (not)
  - You can google logic operator tables for the truth/false equations of expected results [Here’s an example article](https://dev.to/banesag/javascript-logical-operators-and-boolean-values-1l07)
  ##### If / Else Statements
  - If statements check **if** the condition is true it will run the nested code telling it what to do **if** this thing is. **if** the thing is *not* (i.e. if it's false) then the **else** statement will tell the program what to do.

  Example of If / Else statement syntax from the textbook referenced above:
  ```
  var pass = 50;
  var score = 75;
  var msg;

  if (score >= pass) {
    msg = 'Congratulations, you passed!';
  } else {
    msg = 'Have another go.';
  };
  ```

[Back to Home](README.md)