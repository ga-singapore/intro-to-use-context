# ![Intro to JavaScript Functions - Instructor Guide](./assets/hero-instructor-guide.png)

## Overview

In this content students will build:
- Function declarations
- Function expressions
- Arrow function expressions

The remainder of the JavaScript content uses arrow function expressions wherever possible, but given that students will frequently encounter these three types, the syntax for all of them are presented in this module. 

## Parameters and Arguments You Do solution

Here's a potential solution to the Parameters and Arguments You Do:

```javascript
function planetHasWater(planet) {
  if (planet === 'Earth' || planet === 'Mars') {
    console.log(true);
  } else {
    console.log(false);
  }
}

planetHasWater('Earth');   // should print true
planetHasWater('Venus');   // should print false
planetHasWater('Mars');    // should print true
planetHasWater('Jupiter'); // should print false
```

## Return Values

In the [Return Values](../return-values/README.md) content, there is a `compileAndSend` function that has a collection of helper functions:

```javascript 
function compileAndSend() {
  let sales = getSalesData();
  let labor = getLaborCosts();
  let budget = getBudget();
  let report = generateReport(sales, labor, budget);
  sendReport(report);
}

// Run the function
compileAndSend()

/*--- helper functions ---*/

function getSalesData() {
  // code to calculate sales
  return sales;
}

function getLaborCosts() {
  // code to calculate labor costs
  return labor;
}

function getBudget() {
  // code to calculate budget
  return budget;
}

function generateReport(sales, labor, budget) {
  // code to generate report
  return report;
}

function sendReport(report) {
  // code to send the report somewhere
}
```

This is intended to be a high-level view of how functions can be written to create larger applications. It is exceptionally hand-wavey to details. 

This is not intended to be an exercise in writing code that would calculate sales data, labor costs, or budgets. It only demonstrates how writing many smaller functions and composing them together can create code that is easier to read and understand at a high level.

### You Do solution

Here's a potential solution to the Return Values You Do

```javascript
function computeArea(width, height) {
  const area = width * height;
  return `The area of a rectangle with a width of ${width} 
    and a height of ${height} is ${area} square units.`;
}

console.log(computeArea(5, 25));
// Prints: 
// The area of a rectangle with a width of 5 
// and a height of 25 is 125 square units.
```

## Arrow Functions

We highly recommend pointing students to the Level Up content associated with arrow functions (or reviewing that content live) if you want to take advantage of more advanced arrow function features with your group.

### You Do solution

A potential solution to this You Do is:

```javascript
const square = (num) => {
  return num * num;
}
```

### Review Questions

There's a marathon of review questions at the end of this microlesson. You don't have to complete all of these with your students together - maybe consider having them quiz each other in breakout rooms? Maybe have them come to a consensus on the questions assigned to them? Anything goes here, do what feels right for your group!

---

🏗️ Under Construction

We are constantly working to improve our resources for instructors and students.

Have something to contribute to this Instructor Guide? [Let us know](https://git.generalassemb.ly/modular-curriculum-all-courses/universal-resources-internal/blob/main/module-feedback.md).
