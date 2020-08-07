# Read:09 \| Forms and Events
[Textbook](https://www.amazon.com/dp/1118907442/ref=cm_sw_em_r_mt_dp_U_X77.EbAN2ACE2): _Jon Duckett: HTML & CSS_ + JavaScript & jQuery  
*(HTML book: Chapters 7 + 14 | JS book: Chapter 6)*  

---
## HTML | Forms
---

- The `<form>` element in HTML is a parent tag where you can nest various input tags to collect information from the user
- Inputs from the form fields are saved as name/value pairs and sent to the server
- You can connect the `<label>` tag to the `<input>` tags using the input's `id` attribute matching to the label's `for` attribute
- The `<input>` tags contain **very useful** `type` attributes such as: `file`, `submit`, `image`, `hidden`, `text`, `password`, `email`, `radio`, `checkbox`
- The `<form>` element takes two standard attributes: `action` (usually a URL) and `method` (GET/POST)

---
## HTML | Lists, Tables and Forms
---

- There are CSS properties that are specifically designed for lists, tables, and forms, such as `list-style-type: lower-roman;`, which would make the bullets on the list turn into lower-case Roman numerals
- To make sure your table cells are consistent across all browsers, be sure to utilize CSS properties such as `border-spacing`, `border-collapse`, `empty-cells`
- Aligning form controls makes the form easier to use for the user, see the image below for reference:
<img src='images/formcontrolcss.jpg' width='500px'>


---
## JS | Events
---

- **Events** are actions made by the user such as a button click or when a page has loaded
  - Includes key press, mouse scrolls, form submits, focus/blur
- **Binding** dictates the event you are listening for from a specific element
- Events are usually captured in a JS **function** which changes the website in some way and feels dynamic to the user
- Event delegation can be set up for future events that happen in child elements

Traditional DOM **event handler** is set up like this:  
  <img src='images/eventHandler.jpg' width='500px'>

**Event listener** syntax is like this:  
  <img src='images/eventListener.jpg' width='500px'>

  > **NOTE:** The preferred modern method is event listener syntax 

Using an **Event Listener** in JS:   
  <img src='images/eListenerCode.jpg' width='500px'>

[Back to Home](README.md)