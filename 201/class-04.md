# Read:04 \| HTML Links, CSS Layout & JS Functions
[Textbook](https://www.amazon.com/dp/1118907442/ref=cm_sw_em_r_mt_dp_U_X77.EbAN2ACE2): _Jon Duckett: HTML & CSS_ + JavaScript & jQuery  
*(HTML book: Chapters 4 + 15 \| JS book: Chapters 3)*  
Article from Code Fellows: [6 Reasons for Pair Programming](https://www.codefellows.org/blog/6-reasons-for-pair-programming/) 

---
## HTML | Links
---
- Links are created using the HTML element tag `<a href='www.clickhere.com'>Click Here</a>`
- To link to **external** websites use the absolute URL: `href='http://www.officialsite.com'`
- To link to **other pages on Same website** use relative URL: `href='about-us.html'` (without referenceing a folder path infront of the file name dictates the file is in the same folder as our index.html file)
- Different pages on your website should ideally be stored in seperate folders (directories), so the main website has an index.html but the about-us page also has it's own index.html in the about-us directory where the files are stored
- To link an email to start up the users email program use: `href='mailto:me@myemail.org'`
- To link to a **specific** part of the **same page**: `href="#anIdAttributeName"`
- Do get to a specific place on an external link, just do the full link and follow it immediately with `/#idName`
- To have the link open in a **New Window** use the target property in the opening tag like this: `<a href='https://gohere.com' target='_blank'>`

---
## CSS | Layout
---
#### Core Concepts
- All elements are in their own "box" which is either represented as **block-level** (starts on a new line, EX: h1, p, ul, li) or **inline** (immediately following previous thing, EX: img, b, i)
- Block-level elements can be nested, the one wrapped around the outside of anouther would be referred to as the **parent** element.

#### Positiong Schemas
- You can use `position` or `float` property in CSS to position elements
- Normal Flow: each new div starts on a new line below the previous one
- Relative Positioning: pushing the block to the top, right, bottom or left of where it would have been
- Absolute Positioning: taken out of the flow (doesn't impact any other elements) and moves as users scroll up and down the page (often like an overlay)
- Fixed Positioning: like absolute but in relation to window and not element, does not move when page scrolls
- Floating Elements: take out of normal flow and position in far left or right of containing box letting other elements to flow around it

---
## JavaScript | Functions & Variable Scopes
---
- A function is a place for you to group several statements together to perform a specific task and can be reused
- Always use the keyword `function` with a function name like “doMath”
- Functions may or may not take in information, if they do, it is called a parameter
- Call functions with (), Ex: doMath() / if your function used **parameters** you would put those values in the () like this: `doMath(1,3)`
- Use `return` to get a single value from the function (usually paired with a var name) / or the `return` can be assigned to an array to get more than one value as a result
- Function Declaration (can be called before it's been declared) vs. Fucntion Expression (cannot call the function before the interpret has discovered it, and any code before it could potentially alter what goes inside)
- **Local Scope** variables are created *inside* a function and only used in that function
- **Global Scope** variables are *outside* the function and can be used anywhere in the script

---
## Article \| [6 Reasons for Pair Programming](https://www.codefellows.org/blog/6-reasons-for-pair-programming/) by Code Fellows

---
> The best practices for a Software Developer: Iterative loops, Code reviews, Fast feedback, Error checking and linting
#### Pair Programming
- Two roles: **Driver** and the **Navigator**.   
  - Driver is the one typing, handling the mechanics (text editor, switching files, version control and code writing).   
  - Navigator uses words to guide driver but doesn't touch the computer / thinks about the big picture, what comes next, how an algo could be converted to code, scans for typos and bugs (they can use their own computer to google solutions and documentation)
- Six reasons to Pair Program are: Greater efficiency / Engaged collaboration / Learning from fellow students / Social skills / Job Interview readiness / Work environment readiness


[Back to Home](README.md)