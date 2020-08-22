# Read:12 \| Components
Article: [EJS Partials](https://medium.com/@henslejoseph/ejs-partials-f6f102cb7433)     
YouTube: [EJS Paritals Video](https://www.youtube.com/watch?v=3_xEEH4fTEk&t=0s&index=7&list=PL7sCSgsRZ-slYARh3YJIqPGZqtGVqZRGt)    


## Notes from Article: 
- **Partials** is for when you want to *reuse* the **same html** for multiple *views*
- You are basically defining a reusable bundle of code in a file and then reusing it via the file name on whatever other pages you need it
- If you want the **same nav and footer** on every web page, you would make a **partial**
  - Store them in a directory and filename like this: 
    `views/partials/navbar.ejs`
- The `navbar.ejs` would contain just the portion of HTML you'd want inserted on another file, so a `<div>` containing the `<nav>` html (a snippet if you will)
- For a reusable footer, it would be the same, just make a `footer.ejs` file with the HTML you want reused
- You would use the `navbar.ejs` file inside your **templates** like your `home.ejs` 
- To insert the navbar.ejs in your home.ejs, you would use delimiters and it would like like this: 
  - `<%- include('partials/navbar') %>`
  - Place that line where it makes sense in your home.ejs file

> Note about **<%-** vs **<%=** | the **-** is similar to jQueries `.html` method and **=** is like jQueries `.text` method


## Notes from Video: 
- Partials are native in EJS. Uses include navbars and footers that are used in multiple places.
- Partials are like a "sub-layout" that you can call from other EJS templates
- Partials are included with tags like `<%- include('partials/onepartial') %>`



[Back to Home](README.md)