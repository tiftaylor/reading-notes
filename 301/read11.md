# Read:11 \| EJS
YouTube: [Series of EJS Videos](https://www.youtube.com/playlist?list=PL7sCSgsRZ-slYARh3YJIqPGZqtGVqZRGt)     
Documentation: [EJS](http://ejs.co/)   
API Docs: [Google Books](https://developers.google.com/books/docs/v1/using#WorkingVolumes)   


## Notes from [Series of EJS Videos](https://www.youtube.com/playlist?list=PL7sCSgsRZ-slYARh3YJIqPGZqtGVqZRGt)  
- best practice group install after making npm init --> `npm install --save express body-parser cors ejs`
  - `app.set('views', path.join(--dirname, 'views'))` = any views in EJS can concatinate a working directory in views
  - `app.set ('view engine', 'ejs')`
- `index.ejs` is how you'll use **ejs** // it's a file extention for express js "views"
- in your .get callback use `response.render('index');` to render the ejs file in your response
  ```
    response.render('index', {
      foo: 'bar'
    });
    ```
  - this Key: 'Value' pair above is used dynamically like **handlebars** on your **ejs** file like this: 
  `<h1>Hello <%= foo %></h1>` // it'll print "Hello bar" on the website


### Array and For Loop in EJS
- In the **key : value** pair object you can pass the value as string or array of objects with their own key/value pairs
- Here is an array example: 
  ```
  response.render('index', {
    people: [
      {name: 'dave'},
      {name: 'jerry'}
    ]
  })
  ```
- You can type logic in the **ejs** syntax in the index.ejs file like this: 
  ```
  <ul>
    <% for(var person of people) { %>
    <li><%= person.name %></li>
    <% } %>
  </ul>
  ```
  - This will print on the website **dave** and **jerry**


### If/Else in EJS
- ```
  <ul>
    <% for(var person of people) { %>
      <% if(person.name === 'dave') { %>
      <li>This is definitely <%= person.name %>!!</li>
      <% } else { %>
      <li>This is definitely not dave!! This is <%= person.name %></li>
      <% } %>
    <% } %>
  </ul>
  ```

### Layouts in EJS
- `mkdir views ` and add a `layout.ejs` 
- `npm install --save express-ejs-layouts` to use layouts as they are NOT native to express
- On `server.js` be sure to `require('express-ejs-layouts')` and `app.use(expressLayouts);` (lets us use the views in the layouts file)
- in this layout file put the generic html set up elements
- child views will be embedded inside of the layout where it says body
- layouts can be used to store navbars and footers and other common markup

### Partials in EJS

- Partials are native in EJS. Uses include navbars and footers that are used in multiple places.
- Partials are like a "sub-layout" that you can call from other EJS templates
- Partials are included with tags like `<%- include('partials/onepartial') %>`


[Back to Home](README.md)