# Read:13 \| Web Application - Local Storage
[diveinto.html5doctor Article](http://diveinto.html5doctor.com/storage.html) titled: *The Past, Present, and Future of Local Storage for Web Applications*

---
## Web Application | Local Storage
---
- HTML5 Storage (also known as DOM Storage) was designed to try and provide a standarized API for storage across multiple browser types without having to rely on third-party plugins.
- HTML5 Storage is a way for web pages to store key/value pairs on the local client (it's never sent to a remote server)
- Below is a snippet of code from the article on how you could manipulate the data
  ```
  var foo = localStorage.getItem("bar");
  // ...
  localStorage.setItem("bar", foo);

  …could be rewritten to use square bracket syntax instead:

  var foo = localStorage["bar"];
  // ...
  localStorage["bar"] = foo;
  ```
- You can remove things by calling `removeItem()`
- To get the total number of values in a storage area, you can iterate like this:   
  ```
  interface Storage {
    readonly attribute unsigned long length;
    getter DOMString key(in unsigned long index);
  };
  ```
- You can track changes to the storage data and then create functions to save the page data (like if it's a game) and then when they reopen the browser/page it can resume the game with a resume function you create. See the "HTML5 Storage In Action" section for full example
- An advanced competitor is **Indexed Database API** which exposes an *object store* (database with records). Use methods provided by the object store to open a database and go through the records
- This article has several further reading links that are worth checking out if you need more details on any aspesct discussed in the article

[Back to Home](README.md)