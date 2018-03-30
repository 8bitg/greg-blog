---
layout: post
title:  Front End Interview Questions
type: post
published: true
comments: false
---

# Introduction
I've been meeting with a number of interviewers in the last several weeks, so I'll be using this post as a way to organize my responses to likely questions.

## Javascript

1. [Closures](#closures)
2. [Event Bubbling](#event-bubbling)
3. [Event Delegation](#event-delegation)
4. [Apply()](#methods-apply)
5. [Call()](#methods-call)
5. [Bind()](#methods-bind)

<hr>

### Explain Javascript Closures <a id="closures"></a>
Definition: A **closure** is a special kind of **object** that combines a **function** and **the environment** in which the function was created.
The *environment* consists of **any local variables** that were **in scope** at the time of the closure's creation.

#### Simple Closure Example
myFunc is a CLOSURE that incorporates both the displayName function and the "Greg" string which existed when the closure was created.

```Javascript  
function makeFunc() {  
    var name = "Greg";  
    function displayName () {  
        alert(name);  
    }  
    return displayName;  
};  
var myFunc = makeFunc();  
myFunc(); // Fires alert with text "Greg"
```

#### Less Simple Closure Example
makeAdder takes a single argument, x, and returns a new function. This function takes a single argument and returns the sum of x and y.

`makeAdder` is essentially a 'function factory'. It creates functions that do different things.
`add5` and `add10` are both CLOSURES. They share the same function body definition, but store different environments.
In `add5` x=5, but in `add10` x=10.


```javascript
function makeAdder(x) {
    return function(y) {
        return x+y;
    };
};
var add5 = makeAdder(5);
var add10 = makeAdder(10);
console.log(add5(2)); // Outputs 7
console.log(add10(2)); // Outputs 12
```

[Back to Top](#)  

<hr>

### Explain Event Bubbling <a id="event-bubbling"></a>
**Event Bubbling** and **Event Capturing** are two ways of event propagation in the HTML DOM API. When an event occurs in an element that is within another element, and *both* have registered a handle for the event.
**Event Propagation Mode** determines the order in which the elements receive the event.  
<a href="http://javascript.info/tutorial/bubbling-and-capturing" target="_blank">Learn More</a>
 
![Bubbling Model](/assets/eventbubbling.png "Bubbling Model")  
**Bubbling**  
The event is captured and handled by the *innermost* element, then propagated to the outer elements. 

**Capturing or *Trickling*** *Only supported by some browsers*  
The event is captured by the *outermost* element and propagated to the inner elements.

### *BUBBLE UP, TRICKLE DOWN*

[Back to Top](#)  
<hr>

### Explain Event Delegation <a id="event-delegation"></a>
Def: **Event Delegation** is a simple technique by which you add a single event handler to a parent element in order to avoid having to add event handlers to multiple child elements.  

Delegation makes use of **Event Bubbling** and the **target element**.
When an event is triggered on an *element*, like a Mouse Click on a Button, the same event is also triggered on all of that element's ancestors, basically, the explanation for *Event Bubbling*.
The **Target Element** of any event is the *originating* element, in this case *the button*, and is stored in a property of the **event object**.

Using Delegation, it is possible to add an event handler to an element, wait for an event to bubble up from a child, and determine from which element the event originated.

```html
<button id="example-btn">
    <span>Hello World</span>
</button>
```

Given this mark-up and putting an event handler on the button, like so 

```javascript
document.getElementById("example-btn").addEventListener("click", function() {
 console.log("Hello") 
});
```

Clicking on the button will fire the event.  
Clicking on the span will also fire the event.

[Back to Top](#)  
<hr>

### Explain Apply(), Bind() and Call() Methods
### Apply() <a id="methods-apply"></a>

Syntax:  
`function.apply(this.Arg, [argsArray])`

Parameters:   
`thisArg` = the value of `this` provided for the call to **function**.  
`argsArray` = an array-like object specifying the arguments with which **function** should be called.

`apply` is very similar to `call()`, except for the type of arguments that it supports. 
`apply` allows you to use an array literal, eg. `function.apply(this, ['eat', 'banana'])`  
**OR**  
an Array object, eg. `function.apply(this, new Array('eat', 'banana'))`  

Def:  
Using `apply`, you can assign a different `this` object when calling an existing function. `this` refers to the calling object (current object).
With `apply`, you can write a method once and then inherit it in another object, without having to rewrite the method for the new object.

Usage:
Can be used to complete tasks that would otherwise have you looping over arrays.

```javascript
var numbers = [5, 6, 2, 3, 7];
var max = Math.max.apply(null, numbers); // Max value of array
var min = Math.min.apply(null, numbers); // Min value of array
```  

[Back to Top](#)  
<hr>

### Call() <a id="methods-call"></a>
<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/call" target="_blank">Learn More</a>

[Back to Top](#)  
<hr>

### Bind() <a id="methods-bind"></a>
<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/bind" target="_blank">Learn More</a>

[Back to Top](#)  
<hr>

### Get Primes Algorithm

#### Write a javascript function which takes in an integer value and returns back an array of all of the prime numbers which factor out of it. (e.g primeFactors(12) -> [2,3,5,7,11])
```javascript
function getPrimes(max) {
    var temp = [], 
        i, 
        j, 
        primes = [];
        
    for (i = 2; i <= max; ++i) {
        if (!temp[i]) {
            // i has not been marked -- it is prime
            primes.push(i);
            for (j = i << 1; j <= max; j += i) {
                temp[j] = true;
            }
        }
    }
    return primes;
}

console.log(getPrimes(30));
```

[Back to Top](#)  
<hr>
