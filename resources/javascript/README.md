# Javascript Resources

## Items to Note  

**Don't Repeat Yourself** (DRY)  
> Write reusable functions that express a lot in very little code.  

**Do One Thing** (DOT)  
> Each function should only do *one* thing. This will make the function more reusable, readable, and easier to debug.  

**Keep It Simple Stupid** (KISS)  
> Don't create cryptic functions, other people need to be able to read and debug them.  

**Less Is More**  
> Self explainatory  

  

## Functions  


### Function Declaration  

Example  
> `function hello(world) { console.log('hello ' + world); }; `  

> `hello(world);`



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
> ` var hello = function (world) { console.log('hello ' + world); }  `  

> `hello(world);`



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



## Books  
[Javascript for Cats](http://jsforcats.com/)  
[Eloquent Javascript](http://eloquentjavascript.net/)  


## Node.JS  
[Node.JS Documentation](https://nodejs.org/documentation/)  
[NodeSchool](http://nodeschool.io/)  
[LearnYouNode](https://github.com/rvagg/learnyounode)  
[Felix's Node Guide](http://nodeguide.com/)  
[Joyent](https://www.joyent.com/developers/node)  
[Node Cloud (resource directory)](http://www.nodecloud.org/)  
[Node Tuts](http://nodetuts.com/)  
[Node Beginner](http://www.nodebeginner.org/)  
