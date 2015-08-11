---
layout: post
title:  Tons of Front End Questions
type: post
published: true
comments: false
---

#Front-end Job Interview Questions

This file contains a number of front-end interview questions that can be used when vetting potential candidates. It is by no means recommended to use every single question here on the same candidate (that would take hours). Choosing a few items from this list should help you vet the intended skills you require.

**Note:** Keep in mind that many of these questions are open-ended and could lead to interesting discussions that tell you more about the person's capabilities than a straight answer would.

## Table of Contents

  1. [General Questions](#general-questions)
  1. [HTML Questions](#html-questions)
  1. [CSS Questions](#css-questions)
  1. [JS Questions](#js-questions)
  1. [Testing Questions](#testing-questions)
  1. [Performance Questions](#performance-questions)
  1. [Network Questions](#network-questions)
  1. [Coding Questions](#coding-questions)
  1. [Fun Questions](#fun-questions)

## Getting Involved

  1. [Contributors](#contributors)
  1. [How to Contribute](https://github.com/h5bp/Front-end-Developer-Interview-Questions/blob/master/CONTRIBUTING.md)
  1. [License](https://github.com/h5bp/Front-end-Developer-Interview-Questions/blob/master/LICENSE.md)

#### General Questions:

1. What did you learn yesterday/this week?
  * How to use Markdown quickly and efficiently.
  * How easy it is to make a script in Node.
  * How difficult it can be to interact with APIs.  
1. What excites or interests you about coding?
  * **Excited** when I solve a problem and experience an *"ah ha"* moment
  * **Interested** by the number of ways to solve a problem, and the variations in best practices for solving different problems.
1. What is a recent **technical challenge** you experienced and how did you solve it?
  * After working with the newest Backbone, Marionette and Bootstrap on a project, I went back to maintaining sites that were developed several years ago without best-practices in mind. Every task that I work on is a new puzzle to solve. Thankfully JQM keeps their super old documentation on their site.
  * Working with APIs in a side-project has taught me the benefits of collaborating to get over a hurdle and the value of setting reachable goals.
1. What **UI, Security, Performance, SEO, Maintainability or Technology** considerations do you make while building a web application or site?
  * **UI**: Mobile-first design, but avoiding to make the desktop version of an application into a blown-up phone interface.
  * **Security**: Avoiding holding onto users personal information by using OAuth2 for login. 
  * **Performance**: Could load the application by making a call from a CDN to reduce the load on local servers
  * **SEO**: Mild familiarity with Twitter Cards and Open-Graph.
  * **Maintainability**: Using `editorconfig` and JSLint to keep code tidy and keep the style to whatever is comfortable for most devs on the team.
  * **Technology**: Researching the latest/greatest, using the technologies that both fit the app's context and is agreed on by a majority in the team.
1. Talk about your preferred **development environment**.
  * **Hardware**
      * Mac or Linux on a machine that is sturdy and portable.
      * At least 1 large monitor and mouse.
      * Pens and notebooks for stand-up notes and diagrams.
      * Earbuds
      * Caffeine and Water for hydration
  * **Software**
      * Spotify
      * Unix terminal
      * Webstorm, Atom or Sublime Text for IDE
      * iTerm2
      * Browsers: Chrome, Firefox, Safari, IE(usually in VBox)
      * GIMP
      * VirtualBox
      * XCode
      * Android Studio
      * XMind - Mind-Mapping software
1. Which **version control systems** are you familiar with?
  * I've worked with **git** for several years. I'm very comfortable working in/solving issues in that environment
1. Can you describe your **workflow** when you create a web page?
  * Decide on the idea and technical approach.
  * Enter some stories into a Trello board to keep track of future features, future design assets and to get push notifications to see who is working on what stories.
  * Build a simple Node/Express http server to serve the files locally and grab external data, if necessary.
  * Stash all api-keys and important information in a config file and require it into the project, but **never** commit it.
  * Set up the scaffolding for whatever MVC framework I'm using, if the project requires a framework.
  * Build templates / Template logic.
  * Add bugs into the Trello.
  * Have regular stand-ups to keep track of the project, if I'm working with collaborators.
  * **Profit**
1. If you have **5 different stylesheets**, how would you best **integrate them** into the site?
  * **Convert** them to SASS.
  * **Import** the files into a master stylesheet.
  * **Clean** the master stylesheet, removing duplicate IDs and Classes.  
1. Can you describe the difference between progressive enhancement and graceful degradation?
1. How would you optimize a website's assets/resources?
1. How many resources will a browser download from a given domain at a time?
  * What are the exceptions?
1. Name 3 ways to decrease page load (perceived or actual load time).
1. If you jumped on a project and they used tabs and you used spaces, what would you do?
1. Describe how you would create a simple slideshow page.
1. If you could master one technology this year, what would it be?
1. Explain the importance of standards and standards bodies.
1. What is Flash of Unstyled Content? How do you avoid FOUC?
1. Explain what ARIA and screenreaders are, and how to make a website accessible.
1. Explain some of the pros and cons for CSS animations versus JavaScript animations.
1. What does CORS stand for and what issue does it address?
  * **CORS = Cross-Origin Resource Sharing**.
  * Provides a way for **web servers** to support cross-site access controls, which enable **secure cross-site data transfers**.

#### HTML Questions:

1. What does a `doctype` do?
1. What's the difference between standards mode and quirks mode?
1. What's the difference between HTML and XHTML?
1. Are there any problems with serving pages as `application/xhtml+xml`?
1. How do you serve a page with content in multiple languages?
1. What kind of things must you be wary of when design or developing for multilingual sites?
1. What are `data-` attributes good for?
1. Consider HTML5 as an open web platform. What are the building blocks of HTML5?
1. Describe the difference between a `cookie`, `sessionStorage` and `localStorage`.
1. Describe the difference between `<script>`, `<script async>` and `<script defer>`.
1. Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions?
1. What is progressive rendering?
1. Have you used different HTML templating languages before?

#### CSS Questions:

1. What is the difference between classes and ID's in CSS?
1. What's the difference between "resetting" and "normalizing" CSS? Which would you choose, and why?
1. Describe Floats and how they work.
1. Describe z-index and how stacking context is formed.
1. Describe BFC(Block Formatting Context) and how it works.
1. What are the various clearing techniques and which is appropriate for what context?
1. Explain CSS sprites, and how you would implement them on a page or site.
1. What are your favourite image replacement techniques and which do you use when?
1. How would you approach fixing browser-specific styling issues?
1. How do you serve your pages for feature-constrained browsers?
  * What techniques/processes do you use?
1. What are the different ways to visually hide content (and make it available only for screen readers)?
1. Have you ever used a grid system, and if so, what do you prefer?
1. Have you used or implemented media queries or mobile specific layouts/CSS?
1. Are you familiar with styling SVG?
1. How do you optimize your webpages for print?
1. What are some of the "gotchas" for writing efficient CSS?
1. What are the advantages/disadvantages of using CSS preprocessors?
  * Describe what you like and dislike about the CSS preprocessors you have used.
1. How would you implement a web design comp that uses non-standard fonts?
1. Explain how a browser determines what elements match a CSS selector.
1. Describe pseudo-elements and discuss what they are used for. 
1. Explain your understanding of the box model and how you would tell the browser in CSS to render your layout in different box models.
1. What does ```* { box-sizing: border-box; }``` do? What are its advantages?
1. List as many values for the display property that you can remember.
1. What's the difference between inline and inline-block?
1. What's the difference between a relative, fixed, absolute and statically positioned element?
1. The 'C' in CSS stands for Cascading.  How is priority determined in assigning styles (a few examples)?  How can you use this system to your advantage?
1. What existing CSS frameworks have you used locally, or in production? How would you change/improve them?
1. Have you played around with the new CSS Flexbox or Grid specs?
1. How is responsive design different from adaptive design?
1. Have you ever worked with retina graphics? If so, when and what techniques did you use?
1. Is there any reason you'd want to use `translate()` instead of *absolute positioning*, or vice-versa? And why?

#### JS Questions:

1. Explain event delegation
1. Explain how `this` works in JavaScript
1. Explain how prototypal inheritance works
1. What do you think of AMD vs CommonJS?
1. Explain why the following doesn't work as an IIFE: `function foo(){ }();`.
  * What needs to be changed to properly make it an IIFE?
1. What's the difference between a variable that is: `null`, `undefined` or undeclared?
  * How would you go about checking for any of these states?
1. What is a closure, and how/why would you use one?
1. What's a typical use case for anonymous functions?
1. How do you organize your code? (module pattern, classical inheritance?)
1. What's the difference between host objects and native objects?
1. Difference between: `function Person(){}`, `var person = Person()`, and `var person = new Person()`?
1. What's the difference between `.call` and `.apply`?
1. Explain `Function.prototype.bind`.
1. When would you use `document.write()`?
1. What's the difference between feature detection, feature inference, and using the UA string?
1. Explain AJAX in as much detail as possible.
1. Explain how JSONP works (and how it's not really AJAX).
1. Have you ever used JavaScript templating?
  * If so, what libraries have you used?
1. Explain "hoisting".
1. Describe event bubbling.
1. What's the difference between an "attribute" and a "property"?
1. Why is extending built-in JavaScript objects not a good idea?
1. Difference between document load event and document ready event?
1. What is the difference between `==` and `===`?
1. Explain the same-origin policy with regards to JavaScript.
1. Make this work:
```javascript
duplicate([1,2,3,4,5]); // [1,2,3,4,5,1,2,3,4,5]
```
1. Why is it called a Ternary expression, what does the word "Ternary" indicate?
1. What is `"use strict";`? what are the advantages and disadvantages to using it?
1. Create a for loop that iterates up to `100` while outputting **"fizz"** at multiples of `3`, **"buzz"** at multiples of `5` and **"fizzbuzz"** at multiples of `3` and `5`
1. Why is it, in general, a good idea to leave the global scope of a website as-is and never touch it?
1. Why would you use something like the `load` event? Does this event have disadvantages? Do you know any alternatives, and why would you use those?
1. Explain what a single page app is and how to make one SEO-friendly.
1. What is the extent of your experience with Promises and/or their polyfills?
1. What are the pros and cons of using Promises instead of callbacks?
1. What are some of the advantages/disadvantages of writing JavaScript code in a language that compiles to JavaScript?
1. What tools and techniques do you use debugging JavaScript code?
1. What language constructions do you use for iterating over object properties and array items?
1. Explain the difference between mutable and immutable objects.
  * What is an example of an immutable object in JavaScript?
  * What are the pros and cons of immutability?
  * How can you achieve immutability in your own code?
1. Explain the difference between synchronous and asynchronous functions.
1. What is event loop?
  * What is the difference between call stack and task queue?

#### Testing Questions:

1. What are some advantages/disadvantages to testing your code?
1. What tools would you use to test your code's functionality?
1. What is the difference between a unit test and a functional/integration test?
1. What is the purpose of a code style linting tool?

#### Performance Questions:

1. What tools would you use to find a performance bug in your code?
1. What are some ways you may improve your website's scrolling performance?
1. Explain the difference between layout, painting and compositing.

#### Network Questions:

1. Traditionally, why has it been better to serve site assets from multiple domains?
1. Do your best to describe the process from the time you type in a website's URL to it finishing loading on your screen.
1. What are the differences between Long-Polling, Websockets and Server-Sent Events?
1. Explain the following request and response headers:
  * Diff. between Expires, Date, Age and If-Modified-...
  * Do Not Track
  * Cache-Control
  * Transfer-Encoding
  * ETag
  * X-Frame-Options
1. What are HTTP actions? List all HTTP actions that you know, and explain them.

#### Coding Questions:

1. Question: What is the value of `foo`?*

```javascript
var foo = 10 + '20';
```

1. Question: How would you make this work?*

```javascript
add(2, 5); // 7
add(2)(5); // 7
```

1. Question: What value is returned from the following statement?*

```javascript
"i'm a lasagna hog".split("").reverse().join("");
```

1. Question: What is the value of `window.foo`?*

```javascript
( window.foo || ( window.foo = "bar" ) );
```

1. Question: What is the outcome of the two alerts below?*

```javascript
var foo = "Hello";
(function() {
  var bar = " World";
  alert(foo + bar);
})();
alert(foo + bar);
```

1. Question: What is the value of `foo.length`?*

```javascript
var foo = [];
foo.push(1);
foo.push(2);
```

1. Question: What is the value of `foo.x`?*

```javascript
var foo = {n: 1};
var bar = foo;
foo.x = foo = {n: 2};
```

1. Question: What does the following code print?*

```javascript
console.log('one');
setTimeout(function() {
  console.log('two');
}, 0);
console.log('three');
```

#### Fun Questions:

1. What's a cool project that you've recently worked on?
1. What are some things you like about the developer tools you use?
1. Do you have any pet projects? What kind?
1. What's your favorite feature of Internet Explorer?
1. How do you like your coffee?


#### Contributors:

This document started in 2009 as a collaboration of [@paul_irish](https://twitter.com/paul_irish) [@bentruyman](https://twitter.com/bentruyman) [@cowboy](https://twitter.com/cowboy) [@ajpiano](https://twitter.com/ajpiano)  [@SlexAxton](https://twitter.com/slexaxton) [@boazsender](https://twitter.com/boazsender) [@miketaylr](https://twitter.com/miketaylr) [@vladikoff](https://twitter.com/vladikoff) [@gf3](https://twitter.com/gf3) [@jon_neal](https://twitter.com/jon_neal) [@sambreed](https://twitter.com/sambreed) and [@iansym](https://twitter.com/iansym).

It has since received contributions from over [100 developers](https://github.com/h5bp/Front-end-Developer-Interview-Questions/graphs/contributors).