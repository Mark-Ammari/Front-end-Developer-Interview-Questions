---
title: HTML Questions
layout: layouts/page.njk
permalink: /questions/html-questions/index.html
---

* What does a `doctype` do?
      It lets the browser know what document you are using. So for example: The html version we are using.
      
* How do you serve a page with content in multiple languages?
      theres a lot of ways, but the main ways is using the lang attribute for html tag or content-language in the http-header
      
* What kind of things must you be wary of when design or developing for multilingual sites?
- `hreflang` attr in link
- `dir` attr indicating language direction, such as `rtl`
- `<meta charset='UTF-8'>`
- `font-size` for `:lang({language_code})` selectors in 
* What are `data-` attributes good for?
      It is used to store custom data
      
* Consider HTML5 as an open web platform. What are the building blocks of HTML5?

* Describe the difference between a `cookie`, `sessionStorage` and `localStorage`.
- A session storage: stores data only for that session, once the browser tab is closed, the data is deleted.
- A local storage: stores data with no expiration date, meaning that the data is still there when you close the browser
- A cookie: stores data temperarily, so it has an expiration date and can be renews whenever the user sets the cookie.

* Describe the difference between `<script>`, `<script async>` and `<script defer>`.
- Script basically is where you write your javascript 
- Script async downloads the script wether the page loads or not
- Script defer waits for the page to load before rendering the script

* Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions?
      It is generally a good Idea to position css link between the head tag because html and css are simutanously parsed where the html is the structure and css is how you want the page to look, placing it anywhere outside the head tag will make the styling not parse simutanously with the html. Doing this will not style your page the way you want it too. simularly placing the script tag at the end is ideal because you want the page to load before manipulating the dom. If you put it on the top it takes more time to load the page and there wont be any elements to manipulate
      the only time you would put the script tag on top is if you use the defer attribute that states it will download and render the script write after the html finish loading on to the page.
      
* What is progressive rendering?
      It is a technique to find ways to make a web page load faster
      - there is lazy loading where we will load a certain number of objects at a time as the user scrolls
* Why you would use a `srcset` attribute in an image tag? Explain the process the browser uses when evaluating the content of this attribute.
      You would use srcset when you want to serve different images based on the device orientation
* Have you used different HTML templating languages before?
      no
