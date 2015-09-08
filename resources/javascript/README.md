# Javascript Notes  

**Don't Repeat Yourself** (DRY)  
Write reusable functions that express a lot in very little code.  

**Do One Thing** (DOT)  
Each function should only do *one* thing. This will make the function more reusable, readable, and easier to debug.  

**Keep It Simple Stupid** (KISS)  
Don't create cryptic functions, other people need to be able to read and debug them.  

**Less Is More**  
Self explainatory  

  
## Functions  

### Closures  
A _closure_ stores function state, even after the function has returned.  
Commonly used to:  
* give objects data privacy
* feed data to event handlers or callbacks, which might get triggered after the containing function has finished  

### Function Declaration  

Example  
`function hello(world) { console.log('hello ' + world); }; `  


### Function Expression    

The Good  
* Can assign functions to variables the same way values can be assigned to variables.
* Can count on _function expressions_ to follow application logic reliably.
* Will work as expected with a _conditional assignment_.  

The Bad  
* _Function expressions_ create _anonymous functions_ unless you explicitly provide a name.  

Other Items to Note  
* _Function expressions_ assigned to object literals are sometimes called _method literals_.  

Example  
` var hello = function (world) { console.log('hello ' + world); }  `  


### IIFE  
_Immediately Invoked Function Expression_. Pronounced: "_iffy_"  
Often used to create a new scope to encapsulate modules.

Example  
`( function foo() { ... }());`  


### Hoisting  
The illusion that all variable declarations are _"hoisted"_ to the top of the containing function.  
Javascript builds its execution environment in two passes. The declaration pass sets up the runtime environment, where it scans for all variable and function declarations and creates the identifiers. The second is the execution pass.  


### Lambdas  
A _lambda_ is a function used as data. Lambdas can be used as:  
* a parameter for another function  
* the return value of a function  
* anywhere a literal value would be used  
* Frequently confused with anonymous functions, closures, first-class functions, and higher order functions.  

Commonly used to:   
* Perform operations on the other args passed in.
* Attach event handlers for DOM interactions. 
* Pass in a _callback function_ to be executed when the current function is comeplete.
* Wrap existing functions with additional functionality (ie: logging).
* Take a function that requires multiple params, and return a function that requires fewer params.
* Return a function from another function. 

## Compatibility  
[Kangax’ ES6 compatibility table](http://kangax.github.io/compat-table/es6/)  


## Books  
[ES6 - Exploring JS](http://exploringjs.com/es6/)  
[Javascript for Cats](http://jsforcats.com/)  
[JavaScript Allongé](https://leanpub.com/javascriptallongesix/read) | by: _Reg “raganwald” Braithwaite_   
[Eloquent Javascript](http://eloquentjavascript.net/) | by: _Marijn Haverbeke_  
[Human Javascript](http://read.humanjavascript.com/) | by: _Henrik Joreteg_  
[Javascript: The Definitive Guide, 6th Edition](http://shop.oreilly.com/product/9780596805531.do) | by: _David Flanagan_  
[Functional Javascript](http://shop.oreilly.com/product/0636920028857.do) | by: _Michael Fogus_  
[Programming Javascript Applications](http://chimera.labs.oreilly.com/books/1234000000262/index.html) | by: _Eric Elliott_  



## Documentation  
[Mozilla Javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)  


## Node.JS  
[Node.JS Documentation](https://nodejs.org/documentation/)  
[NodeSchool](http://nodeschool.io/)  
[LearnYouNode](https://github.com/rvagg/learnyounode)  
[Felix's Node Guide](http://nodeguide.com/)  
[Joyent](https://www.joyent.com/developers/node)  
[Node Cloud (resource directory)](http://www.nodecloud.org/)  
[Node Tuts](http://nodetuts.com/)  
[Node Beginner](http://www.nodebeginner.org/)  
