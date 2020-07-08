# Read:05 \| HTML Images, CSS Color & Text
[Textbook](https://www.amazon.com/dp/1118907442/ref=cm_sw_em_r_mt_dp_U_X77.EbAN2ACE2): _Jon Duckett: HTML & CSS_ + JavaScript & jQuery  
*(HTML book: Chapters 5, 11, 12)* 

---
## HTML | Images
---

- Boost appeal of the website
- Image files should be stored in an image folder in your project repo
Image Tag for HTML: 
`<img src=’images/dog.jpg‘ alt=’Dog Photo’ title=’This dog is the cutest‘>`
- You can adjust images using `height` or `width` (and `align`) directly in the img tag or on the css file
- Placement of your tag akin to other tags will determine if it falls above, inline or in the middle of something
> Success Tips: Save img in right **format**, save img in right **size**, and measure the img in **pixels**

- JPG is good for img with lots of colors, PNG/GIF is good for simple colored images
- **vector** imgs are resolution-independent
- To have a caption at the bottom of the image you can put the `img` tag inside of a `<figure>` tag including a `<br>` and the `<figcaption>` tag


---
## CSS | Color & Text
---

#### Color
- Important for setting the mood / theme for the intention of your page
- You can specify using **RGB**, **Hex codes**, and **color names** and **HSL**
- Pay attention to contrast
- You can tag on a number at end of RGB to dictate opacity  
> [Google Search](https://www.google.com/search?q=color+picker&oq=color+picker&aqs=chrome..69i57j46j69i65l2j69i60l2j69i65j69i60.1224j0j1&sourceid=chrome&ie=UTF-8) offers a great in-search Color Picker

#### Text
- Main types of text are: **serif**, **sans-serif**, **monospace**, **cursive** and **fantasy** which can be manipulated via font **weight**, **style** and **stretch**
	- Note: Not all fonts will render the same in a person's browser unless you have hardcoded a link to the font in your html file
- You can alter size by **pixels**, **percentages**, and **ems**/**rems** 
- You can also respond to a users mouse/keyboard by using pseudo-classes like `:hover`, `:active` and `:focus`


[Back to Home](README.md)