---
title: CSS Questions
layout: layouts/page.njk
permalink: /questions/css-questions/index.html
---

* What is CSS selector specificity and how does it work?
      specificity is a set of rules that css abids by. the more specific the selector is the more it will not be overrided by other selectors. the heirarchy is as follows inline, then id, then class, then element
      
* What's the difference between "resetting" and "normalizing" CSS? Which would you choose, and why?
      Resetting means you are able to override the original style set on the html element whereas normalisation is what you see is what you get 
      
* Describe Floats and how they work.
      It positions elements to the left or right side of the page. This is an example of a poor mans gridbox
      
* Describe z-index and how stacking context is formed.
      z-index essentially tells the browser which element should be in the front or back.
      
* Describe BFC (Block Formatting Context) and how it works.
      determine what positioning and clearing should be done

* What are the various clearing techniques and which is appropriate for what context?
      we can use clear: both or overflow: auto to fix the problem
      
* How would you approach fixing browser-specific styling issues?
      theres alot of ways we can do this we can create a new stylesheet just for that browser or we can use css frameworks and that will take care of the problem as a whole
      
* How do you serve your pages for feature-constrained browsers?
  * What techniques/processes do you use?
        Graceful degradation: The practice of building an application for modern browsers while ensuring it remains functional in older browsers.
Progressive enhancement: The practice of building an application for a base level of user experience, but adding functional enhancements when a browser supports it.

* What are the different ways to visually hide content (and make it available only for screen readers)?
      visibility: hidden;
      width: 0; height: 0;
      position; absolute; left: -9999px
      
* Have you ever used a grid system, and if so, what do you prefer?
     
* Have you used or implemented media queries or mobile specific layouts/CSS?
      
* Are you familiar with styling SVG?

* Can you give an example of an `@media` property other than `screen`?
      theres all that is used for all media type devices, theres printer used for printers and theres speech used for screenreaders
      
* What are some of the "gotchas" for writing efficient CSS?
      try to reuse styles, try to use class and id selectors more, try to avoid using universal selector, keep in mind of specificity
      
* What are the advantages/disadvantages of using CSS preprocessors?
  * Describe what you like and dislike about the CSS preprocessors you have used.
        You can declare variables that you can use throughout your code, you can have nested elements, have mathmatical functions
        one disadvantage is that it is a compiler so it will take time to render to the page
        
* How would you implement a web design comp that uses non-standard fonts?
      You can use link to link to any font api and use font-family to change the font, you can use @import in css to import fonts
      
* Explain how a browser determines what elements match a CSS selector.
* Describe pseudo-elements and discuss what they are used for.
       pseudo-selector is a keyword added next to the selector to let you style a secific part of the element a good example is :hover or :first-letter or :last-letter
       
* Explain your understanding of the box model and how you would tell the browser in CSS to render your layout in different box models.
      he box model consist of its content with a width and a height, then the padding, then the border, then the margin. naturally, if we dont specify the height or width of the content, then it is only as high and wide as the content is where the height will have some padding and the width wont have any padding.
* What does ```* { box-sizing: border-box; }``` do? What are its advantages?
* What is the CSS `display` property and can you give a few examples of its use?
      none, block, inline, inline-block, flex, grid, table, 
* What's the difference between inline and inline-block?
        with inline you cant specify a width and a height and inline-block you can
* What's the difference between the "nth-of-type()" and "nth-child()" selectors?
* What's the difference between a relative, fixed, absolute and statically positioned element?
* What existing CSS frameworks have you used locally, or in production? How would you change/improve them?
* Have you played around with the new CSS Flexbox or Grid specs?
* Can you explain the difference between coding a web site to be responsive versus using a mobile-first strategy?
* Have you ever worked with retina graphics? If so, when and what techniques did you use?
* Is there any reason you'd want to use `translate()` instead of *absolute positioning*, or vice-versa? And why?
