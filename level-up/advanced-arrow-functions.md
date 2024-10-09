# ![Intro to JavaScript Functions - Level Up - Advanced Arrow Functions](./assets/hero-advanced-arrow-functions.png)

**Learning Objective:** By the end of this lesson, students will be able to optimize arrow functions through the use of implicit returns and single parameter syntax, while understanding the limitations associated with the `this` keyword.

## Implicit return

Arrow functions composed of a single expression (something resolves to a single value) will automatically evaluate and return that expression without requiring us to write the `return` keyword. Just leave off the curly braces, and the rest happens automatically.

```javascript
const multiply = (numA, numB) => numA * numB;

console.log(multiply(3, 4));
// Prints: 12
```

## Single parameters

When working with a single parameter, we can omit the parentheses entirely:

```javascript
// note the lack of () around the num parameter!
const addTwo = num => {
  console.log(num + 2);
}

addOne(2);
```

## Combining these ideas

Here's an example combining both of the above concepts and using them in a single function:
```javascript
const double = num => num * 2;
```

## Arrow function pitfalls

Arrow Functions have a unique way of binding the `this` keyword, which makes them unsuitable for use as object methods or constructors - but don't worry too much about that for now.
