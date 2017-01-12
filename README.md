#Front-end Job Interview Questions

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

## Credit

  1. [Written By](#contributors)
  1. [License](https://github.com/h5bp/Front-end-Developer-Interview-Questions/blob/master/LICENSE.md)

#### General Questions:

* What did you learn yesterday/this week?
  - 1/11/17: I got the flu this week, but I did learn more about how handlers work in Google App Engine.
* What excites or interests you about coding?
  - I love the immediate reward that solving problems gives you in computer science as opposed to physics or math, where results can take longer to interpret or may be ambiguous.
* What is a recent technical challenge you experienced and how did you solve it? 
  - I had to create separate comment and like functions in Google App Engine for my blog project, and kept facing debugging issues. I went back to the basics, simplified my project and my understanding of handlers and got it back working by separating everything into classes instead of handlers.
* What UI, Security, Performance, SEO, Maintainability or Technology considerations do you make while building a web application or site?
  - UI: Less is more. To draw on Roman Mars, design is 99% invisible. The user should not even notice how easy your site is to use, unless they reflect on it.
  - Security: Security is a game of always staying ahead of trends. I try to read on best current practices often and implement them.
  - SEO: I study similar competitors, see where their backlinks are coming from, how they are formatting things. It's not about stealing, but about understanding how they optimize their searchability.
  - Performance: Javascript and media are the biggest slow-downs, and are the primary focuses of optimization. JS must be merged and minified where possible, and images have to be optimized. I also believe in rendering only the best image necessary for the device resolution.
  - Maintainability: Commenting, consistency, and immutability.
  - Technology: Whatever does the job. This means whatever does the job **and** is used by my collaborators.
* Talk about your preferred development environment.
  - I prefer Mac, but I have an XPS 13, which isn't so bad.
  - I use Sublime Text, Spyder and Chrome Canary.
* Which version control systems are you familiar with?
  - Github
* Can you describe your workflow when you create a web page?
  - Testing after each step: Create Google App project, create configuration files (.yaml), then create main python file with handlers. Create Jinja framework helpers to speed up coding. Create template HTML files and load in Bootstrap. Create additional CSS file for further theming. Create handlers and other functions as needed in Python until web page is performing as desired, creating necessary HTML structures as required to test. Lastly, create any additional HTML structures, text, images, and styling. After this, it's testing, security, optimization, SEO, etc.
* If you have 5 different stylesheets, how would you best integrate them into the site?
  - I would probably merge them and minify them using Grunt.
* Can you describe the difference between progressive enhancement and graceful degradation?
  - Progressive Enhancement is the process of slowly adding cutting edge features to your website while not breaking it. Graceful Degradation is the process of trying to ensure your website will still at least marginally function even on the oldest browsers, using workarounds should your modern features fail.
* How would you optimize a website's assets/resources?
  - I answered this for an earlier question.
* How many resources will a browser download from a given domain at a time?
  - 6
  * What are the exceptions?
    - Firefox will do 8
* Name 3 ways to decrease page load (perceived or actual load time).
  - Limit @media requests
  - Limit number of script calls by merging files (and minifying them)
  - Optimize image and media files
* If you jumped on a project and they used tabs and you used spaces, what would you do?
  - I would have to suck it up and use tabs, which are better.
* Describe how you would create a simple slideshow page.
  - I would use SlidesJS for JQuery. No reason to reinvent the wheel and waste my employer's time.
* If you could master one technology this year, what would it be?
  - I definitely want to master more than one this year! .NET, VB, Haskell and Flask are a few that I want to master this month.
* Explain the importance of standards and standards bodies.
* What is Flash of Unstyled Content? How do you avoid FOUC?
  - That gross moment where none of the text is wearing clothes... I mean, styles. You can avoid this by loading scripts with "async" enabled, and by placing them in `<head>`.
* Explain what ARIA and screenreaders are, and how to make a website accessible.
  - Accessible Rich Internet Applications and screenreaders are the only way differently abled people access the web. This can mean no Ajax, no dynamicism, and many images are unavailable to them. One way to combat this is by using modern HTML `<section>`, `<header>`, and other semantic tags, as well as providing `alt` tags, and simplifying overall site structure to be more screenreader-friendly. However, this is not enough. With WAI-ARIA, you can also supply roles for complex navigation techniques and APIs, making this framework exciting and necessary. I am passionate about accessibility because of the friends I made in college, who needed special accomodations while also taking a special place in my heart, and I will fight for their right to browse. My first web development job was in making a department website screenreader friendly.
* Explain some of the pros and cons for CSS animations versus JavaScript animations.
  - CSS is more CPU-efficient, and doesn't require a JavaScript call. However, CSS is not logic friendly, while JavaScript is a logic language.
* What does CORS stand for and what issue does it address?
  - Cross Origin Resource Sharing is primarily a JavaScript concept that seeks to ignore browsers' built-in protection against script-originated cross-domain resource requests. You would do this if you wanted to use multiple servers.
#### HTML Questions:

* What does a `doctype` do?
  - `doctype` tells legacy browsers what language the webpage was written in.
* What's the difference between full standards mode, almost standards mode and quirks mode?
  - These three modes were implemented because when the W3 standards were created, it took a long time for most sites to start meeting the standards, and browsers didn't want to break the internet. These modes instead are the browser's "guess" as to how "quirky" the website is, that is, how poorly it fits the current standards, in order to render a consistent user experience.
* What's the difference between HTML and XHTML?
  - XHTML is eXtensible HTML, is stricter than HTML, and is based on XML instead of SGML.
* Are there any problems with serving pages as `application/xhtml+xml`?
  - Early versions of IE will not recognize them as webpages.
* How do you serve a page with content in multiple languages?
  - You can use META tags or `lang` to specify the languages.
* What kind of things must you be wary of when design or developing for multilingual sites?
  - Some of the same issues any time you change text, including accomodating varying line and words lengths.
  - Setting `charset` to UTF-8.
  - `dir` and `hreflang` attributes to specify the language direction and link language.
* What are `data-` attributes good for?
  - *Not yet answered*
* Consider HTML5 as an open web platform. What are the building blocks of HTML5?
  - *Not yet answered*
* Describe the difference between a `cookie`, `sessionStorage` and `localStorage`.
  - *Not yet answered*
* Describe the difference between `<script>`, `<script async>` and `<script defer>`.
  - *Not yet answered*
* Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions?
  - *Not yet answered*
* What is progressive rendering?
  - *Not yet answered*
* Have you used different HTML templating languages before?
  - *Not yet answered*

#### CSS Questions:

* What is the difference between classes and IDs in CSS?
  - *Not yet answered*
* What's the difference between "resetting" and "normalizing" CSS? Which would you choose, and why?
  - *Not yet answered*
* Describe Floats and how they work.
  - *Not yet answered*
* Describe z-index and how stacking context is formed.
* Describe BFC(Block Formatting Context) and how it works.
* What are the various clearing techniques and which is appropriate for what context?
* Explain CSS sprites, and how you would implement them on a page or site.
* What are your favourite image replacement techniques and which do you use when?
* How would you approach fixing browser-specific styling issues?
* How do you serve your pages for feature-constrained browsers?
  * What techniques/processes do you use?
* What are the different ways to visually hide content (and make it available only for screen readers)?
* Have you ever used a grid system, and if so, what do you prefer?
* Have you used or implemented media queries or mobile specific layouts/CSS?
* Are you familiar with styling SVG?
* How do you optimize your webpages for print?
* What are some of the "gotchas" for writing efficient CSS?
* What are the advantages/disadvantages of using CSS preprocessors?
  * Describe what you like and dislike about the CSS preprocessors you have used.
* How would you implement a web design comp that uses non-standard fonts?
* Explain how a browser determines what elements match a CSS selector.
* Describe pseudo-elements and discuss what they are used for.
* Explain your understanding of the box model and how you would tell the browser in CSS to render your layout in different box models.
* What does ```* { box-sizing: border-box; }``` do? What are its advantages?
* List as many values for the display property that you can remember.
* What's the difference between inline and inline-block?
* What's the difference between a relative, fixed, absolute and statically positioned element?
* The 'C' in CSS stands for Cascading.  How is priority determined in assigning styles (a few examples)?  How can you use this system to your advantage?
* What existing CSS frameworks have you used locally, or in production? How would you change/improve them?
* Have you played around with the new CSS Flexbox or Grid specs?
* How is responsive design different from adaptive design?
* Have you ever worked with retina graphics? If so, when and what techniques did you use?
* Is there any reason you'd want to use `translate()` instead of *absolute positioning*, or vice-versa? And why?

#### JS Questions:

* Explain event delegation
* Explain how `this` works in JavaScript
* Explain how prototypal inheritance works
* What do you think of AMD vs CommonJS?
* Explain why the following doesn't work as an IIFE: `function foo(){ }();`.
  * What needs to be changed to properly make it an IIFE?
* What's the difference between a variable that is: `null`, `undefined` or undeclared?
  * How would you go about checking for any of these states?
* What is a closure, and how/why would you use one?
* What's a typical use case for anonymous functions?
* How do you organize your code? (module pattern, classical inheritance?)
* What's the difference between host objects and native objects?
* Difference between: `function Person(){}`, `var person = Person()`, and `var person = new Person()`?
* What's the difference between `.call` and `.apply`?
* Explain `Function.prototype.bind`.
* When would you use `document.write()`?
* What's the difference between feature detection, feature inference, and using the UA string?
* Explain Ajax in as much detail as possible.
* What are the advantages and disadvantages of using Ajax?
* Explain how JSONP works (and how it's not really Ajax).
* Have you ever used JavaScript templating?
  * If so, what libraries have you used?
* Explain "hoisting".
* Describe event bubbling.
* What's the difference between an "attribute" and a "property"?
* Why is extending built-in JavaScript objects not a good idea?
* Difference between document load event and document DOMContentLoaded event?
* What is the difference between `==` and `===`?
* Explain the same-origin policy with regards to JavaScript.
* Make this work:
```javascript
duplicate([1,2,3,4,5]); // [1,2,3,4,5,1,2,3,4,5]
```
* Why is it called a Ternary expression, what does the word "Ternary" indicate?
* What is `"use strict";`? what are the advantages and disadvantages to using it?
* Create a for loop that iterates up to `100` while outputting **"fizz"** at multiples of `3`, **"buzz"** at multiples of `5` and **"fizzbuzz"** at multiples of `3` and `5`
* Why is it, in general, a good idea to leave the global scope of a website as-is and never touch it?
* Why would you use something like the `load` event? Does this event have disadvantages? Do you know any alternatives, and why would you use those?
* Explain what a single page app is and how to make one SEO-friendly.
* What is the extent of your experience with Promises and/or their polyfills?
* What are the pros and cons of using Promises instead of callbacks?
* What are some of the advantages/disadvantages of writing JavaScript code in a language that compiles to JavaScript?
* What tools and techniques do you use debugging JavaScript code?
* What language constructions do you use for iterating over object properties and array items?
* Explain the difference between mutable and immutable objects.
  * What is an example of an immutable object in JavaScript?
  * What are the pros and cons of immutability?
  * How can you achieve immutability in your own code?
* Explain the difference between synchronous and asynchronous functions.
* What is event loop?
  * What is the difference between call stack and task queue?
* Explain the differences on the usage of `foo` between `function foo() {}` and `var foo = function() {}`

#### Testing Questions:

* What are some advantages/disadvantages to testing your code?
* What tools would you use to test your code's functionality?
* What is the difference between a unit test and a functional/integration test?
* What is the purpose of a code style linting tool?

#### Performance Questions:

* What tools would you use to find a performance bug in your code?
* What are some ways you may improve your website's scrolling performance?
* Explain the difference between layout, painting and compositing.

#### Network Questions:

* Traditionally, why has it been better to serve site assets from multiple domains?
* Do your best to describe the process from the time you type in a website's URL to it finishing loading on your screen.
* What are the differences between Long-Polling, Websockets and Server-Sent Events?
* Explain the following request and response headers:
  * Diff. between Expires, Date, Age and If-Modified-...
  * Do Not Track
  * Cache-Control
  * Transfer-Encoding
  * ETag
  * X-Frame-Options
* What are HTTP methods? List all HTTP methods that you know, and explain them.

#### Coding Questions:

*Question: What is the value of `foo`?*
```javascript
var foo = 10 + '20';
```

*Question: How would you make this work?*
```javascript
add(2, 5); // 7
add(2)(5); // 7
```

*Question: What value is returned from the following statement?*
```javascript
"i'm a lasagna hog".split("").reverse().join("");
```

*Question: What is the value of `window.foo`?*
```javascript
( window.foo || ( window.foo = "bar" ) );
```

*Question: What is the outcome of the two alerts below?*
```javascript
var foo = "Hello";
(function() {
  var bar = " World";
  alert(foo + bar);
})();
alert(foo + bar);
```

*Question: What is the value of `foo.length`?*
```javascript
var foo = [];
foo.push(1);
foo.push(2);
```

*Question: What is the value of `foo.x`?*
```javascript
var foo = {n: 1};
var bar = foo;
foo.x = foo = {n: 2};
```

*Question: What does the following code print?*
```javascript
console.log('one');
setTimeout(function() {
  console.log('two');
}, 0);
console.log('three');
```

#### Fun Questions:

* What's a cool project that you've recently worked on?
* What are some things you like about the developer tools you use?
* Who inspires you in the front-end community?
* Do you have any pet projects? What kind?
* What's your favorite feature of Internet Explorer?
* How do you like your coffee?


#### Contributors:

This document started in 2009 as a collaboration of [@paul_irish](https://twitter.com/paul_irish) [@bentruyman](https://twitter.com/bentruyman) [@cowboy](https://twitter.com/cowboy) [@ajpiano](https://twitter.com/ajpiano)  [@SlexAxton](https://twitter.com/slexaxton) [@boazsender](https://twitter.com/boazsender) [@miketaylr](https://twitter.com/miketaylr) [@vladikoff](https://twitter.com/vladikoff) [@gf3](https://twitter.com/gf3) [@jon_neal](https://twitter.com/jon_neal) [@sambreed](https://twitter.com/sambreed) and [@iansym](https://twitter.com/iansym).

It has since received contributions from over [100 developers](https://github.com/h5bp/Front-end-Developer-Interview-Questions/graphs/contributors).
