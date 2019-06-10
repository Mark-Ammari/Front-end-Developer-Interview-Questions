---
title: JavaScript Questions
layout: layouts/page.njk
permalink: /questions/javascript-questions/index.html
---

* Explain event delegation.
      When an event is fired from an element, the event will be bubbled up to its parent nodes. However, the original element where the event occurs, called 'target', stays the same in the event object. Using the target property, we can always keep tracking which element actually causes an event captured by its parent, and it can help use reduce the number of event handlers as we sometimes don't need to add event listeners for every element.

* Explain how `this` works in JavaScript.
      `this` could refer to multiple things for instance it can refer to a global object such as a variable outside or a winow object and in an event handler it will refer to the element itself 
  * Can you give an example of one of the ways that working with `this` has changed in ES6?
        this regers to a variable created in the function instead of referencing an object outside the function
        
* Explain how prototypal inheritance works.
      prototypes are functions or objects that a class inherit, the point of this is to not repeat ourselves and to have distinct classes.
* What's the difference between a variable that is: `null`, `undefined` or undeclared?
      null means that the variable doesn't exist yet, undefined means that that a variable is declared but it is not referencing to anything, undeclared means a variable that is declared without the var, let, or const
      
  * How would you go about checking for any of these states?
* What is a closure, and how/why would you use one?
      closure is a function within a fuction, where the inner function can access a variable from the outer function
* What language constructions do you use for iterating over object properties and array items?
* Can you describe the main difference between the `Array.forEach()` loop and `Array.map()` methods and why you would pick one versus the other?
      foreach iterates through each element of the array whereas mapping will create a new array and copy the values of that array without effecting the state of the old array
* What's a typical use case for anonymous functions?
      pass them as arguments
      
* What's the difference between host objects, and built-in objects user objects?
      host objects are the window, built-in objects are objects the are supplied by the js library and user objects is what we create
* Explain the difference between: `function Person(){}`, `var person = Person()`, and `var person = new Person()`?
      - declaring a new class
      - declaring a varible that is assigned to that Person()
      - declaring a variable that creates a new instance of Person()
      
* Explain the differences on the usage of `foo` between `function foo() {}` and `var foo = function() {}`
      - creating a function declaration
      - creating a function expression
      
* Can you explain what `Function.call` and `Function.apply` do? What's the notable difference between the two?
* Explain `Function.prototype.bind`.
      bind creates a new function that will have the this keyword set to the first param
      
* What's the difference between feature detection, feature inference, and using the UA string?
      feature detection is checking if a feature exist in a browser
      feature inference means you know a feature exist so you assume that new gen web tech will work
      UA string is info about the browser environment
      
* Explain "hoisting".
       a variable can be declared after it has been used
       
* Describe event bubbling.
       with event bubbling is captured and handled by the innermost element and propagates to the outermost element
       
* Describe event capturing.
       with event capturing it captures the outermost element and trickles down to the innermost element
       
* What's the difference between an "attribute" and a "property"?
      attribute is additional info whereas property is the characteristics
      
* What are the pros and cons of extending built-in JavaScript objects?

* What is the difference between `==` and `===`?
      == double equals doesnt take into consideration datatype while triple equals does
      
* Explain the same-origin policy with regards to JavaScript.
      its an extra security measure taken to restrict how a document is loaded from one place to another
* Why is it called a Ternary operator, what does the word "Ternary" indicate?
* What is strict mode? What are some of the advantages/disadvantages of using it?
       use strict prevents developers writing bad syntax by creating real errors for bad syntax
       
* What are some of the advantages/disadvantages of writing JavaScript code in a language that compiles to JavaScript?
        advantage: utilize new gen js, disadvantage it is slower because it takes an extra step
        
* What tools and techniques do you use debugging JavaScript code?
        
* Explain the difference between mutable and immutable objects.
      mutable means an objects state can be changed and immutable means an objects state cannot be changed
  * What is an example of an immutable object in JavaScript?
        integer or string is immutable
  * What are the pros and cons of immutability?
        you cant change the state of your data so it makes your code more strict and secure.
  * How can you achieve immutability in your own code?
        using const or object.assign
        
* Explain the difference between synchronous and asynchronous functions.
        async simply means while a function is running and it consumes alot of time it will run as a daemon process and execute the async function while a sync funtion has to wait for all the task before it to finish before executing.
        
* What is event loop?
      
  * What is the difference between call stack and task queue?
        call stack keep track of function calls when we call a function for execution an pop it out once were done
        task queue
* What are the differences between variables created using `let`, `var` or `const`?
      let is block scoped meaning that it can not be refered outside of the scope it is in
      var is lexically scoped meaning that it can be refered outside of the scope it is in
      const means the value does not change
      
* What are the differences between ES6 class and ES5 function constructors?
* Can you offer a use case for the new arrow `=>` function syntax? How does this new syntax differ from other functions?
      they are great for creating shorthand functions
* What advantage is there for using the arrow syntax for a method in a constructor?
* What is the definition of a higher-order function?
      takes functions as arguments or returns a function
      
* Can you give an example for destructuring an object or an array?
      const person = { first: "mark", last: "ammari" }
      const {first, last} = person
      console.log(first, last)
* Can you give an example of generating a string with ES6 Template Literals?
      ${name} (interpolation)
      \n (new line)

* Can you give an example of a curry function and why this syntax offers an advantage?
      Currying is a process in functional programming in which we can transform a function with multiple arguments into a sequence of nesting functions. It returns a new function that expects the next argument inline.
      
* What are the benefits of using `spread syntax` and how is it different from `rest syntax`?
      spread ads array elements to an existing array
      rest you can add as many arguments as you want
      
* How can you share code between files?
      you would export the function to be used in another java script file
      
* What is encapsulation?
      wrapping all your variables and functions in the same location that are related to each other
      
* what is abstraction?
        hide all the nasty complexity and only show the essentials.
        
* What is polymorphism
      allows us to get rid of if el and switch cases
      
* What is a factory function?
      create objects for you so you dont have to repeat yourself



## Coding questions
* Make this work:
```javascript
duplicate([1,2,3,4,5]); // [1,2,3,4,5,1,2,3,4,5]
```
* Create a for loop that iterates up to `100` while outputting **"fizz"** at multiples of `3`, **"buzz"** at multiples of `5` and **"fizzbuzz"** at multiples of `3` and `5`
