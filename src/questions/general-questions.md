---
title: General Questions
layout: layouts/page.njk
permalink: /questions/general-questions/index.html
---

* When building a new web site or maintaining one, can you explain some techniques you have used to increase performance?
      try not to use compilers, use lazy loading approach
      
* Can you describe some SEO best practices or techniques you have used lately?
      using meta tags
      
* Can you explain any common techniques or recent issues solved in regards to front-end security?
      cors
      
* What actions have you personally taken on recent projects to increase maintainability of your code
      make it easy to read, reuse code instead of creating redundant code, constantly update your code
      
* Which version control systems are you familiar with?
      version control lets you know the risk and priorities to update your code a good version control is git
      
* Can you describe your workflow when you create a web page?
      first I go to the drawing board to visualize how I want my page to look like
      
* If you have 5 different stylesheets, how would you best integrate them into the site?
      we can use a css preprocessor to import them as partials so that way we control what gets styled from a central styling file instead of importing multiple files
      
* Can you describe the difference between progressive enhancement and graceful degradation?

* How would you optimize a website's assets/resources?
      we can import a sprite sheet instead of a bunch of static images and by doing so we are able to reduce
      
* How many resources will a browser download from a given domain at a time?
      it depends on the browser but the modern browser would support concurrent downloads
      
  * What are the exceptions?
* Name 3 ways to decrease page load (perceived or actual load time).
      Reduce perceived download time: Add a some visual feedback, either a spinner or an actual progress, bar that displays during page load.
      Load static content first: Ensure that static page content loads first and then load additional assets in the background afterwards.
      Reduce the quantity of items to load:  Eg combine all js files into a single file, all css files into a single file, etc), to reduce the number of requests that the browser needs to make.
      
* If you jumped on a project and they used tabs and you used spaces, what would you do?
      I would use tabs because you should always follow the coding convention of a company.
      
* Describe how you would create a simple slideshow page.

* If you could master one technology this year, what would it be?

* Explain the importance of standards and standards bodies.

* What is Flash of Unstyled Content? How do you avoid FOUC?
      this usually happens when the html and css are not parsed simultaniously, to prevent this we have to put a link tag in the head
      
* Explain what ARIA and screenreaders are, and how to make a website accessible.
      its ways to make our website more accessible to people with disabilities. aria is accessible rich internet application and its practices using attributes to give semantic meaning to our page.
      
* Explain some of the pros and cons for CSS animations versus JavaScript animations.
      CSS animations dont disrupt the normal flow of the page
      javascript has advanced animations like bouncing and pulsating
      with javascript you have more control with animation
      css its small and simple.
        
* What does CORS stand for and what issue does it address?
      cors stand for cross origin resource sharing and it addresses who gets access to what resources. the reason why apis have cors is to prevent users from manipulating data that is not theirs. Usually when making a request you're required to use an api key in your http header in order to access and ofen times you are limited to just accessing data.
      
* How did you handle a disagreement with your boss or your collaborator?

* What resources do you use to learn about the latest in front end development and design?
