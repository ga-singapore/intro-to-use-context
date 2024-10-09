# ![Intro to JavaScript Functions - Level Up - Fewer Arguments than Parameters](./assets/hero-fewer-arguments-than-parameters.png)

**Learning Objective:** By the end of this lesson, the learner will be able to identify and explain the behavior of JavaScript functions when invoked with fewer arguments than the defined parameters, including how missing arguments default to undefined.

JavaScript is very flexible and won't complain when the number of arguments differs from the number of parameters defined.

If fewer arguments are passed than parameters defined, the parameter variables without a matching argument would be `undefined`.

```javascript
const add = (numA, numB, numC) => {
  return numA + numB + numC;
}

console.log(add(5, 2));
// Prints: NaN
```

Unlike other programming languages, JavaScript won't complain if fewer (or extra) arguments are passed to a function. However, a function that depends on certain arguments to do its job might throw an error or return an unexpected result, like the example above.
