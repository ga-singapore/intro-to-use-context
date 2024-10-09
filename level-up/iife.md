# ![Intro to JavaScript Functions - Level Up - IIFEs](./assets/hero-iifes.png)

**Learning Objective:** Understand how to use Immediately Invoked Function Expressions (IIFEs) to encapsulate variables and prevent them from entering the global scope.

One of the ways we can prevent our code from leaking into the global scope is by wrapping it with a construct known as an Immediately Invoked Function Expression, or IIFE (pronounced iffy). It looks like this:

```javascript
(() => {
  'use strict';

  // your code here
	
})()
```

Wrapping the function in parenthesis (this is a [grouping operator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Grouping) that acts as a container for the function) and invoking it means that it is exected right when it's defined.
