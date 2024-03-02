---
description: >-
  Learning Objectives: Grasp and apply JavaScript syntax and foundational
  programming concepts. Understand variables, different data types, and
  operators. Learn to write and invoke basic functions.
---

# JavaScript Basics

* **Introduction to JavaScript:**
  * _Purpose:_ Discuss JavaScript's role in adding interactivity to web pages and its evolution into a tool for both client-side and server-side development.
* **Variables and Data Types:**
  * _Variables:_ Introduction to `let` and `const` for declaring variables.

{% code overflow="wrap" fullWidth="false" %}
```javascript
let message = "Hello, JavaScript!"; 
const pi = 3.14;
```
{% endcode %}

* _Data Types:_ Explore strings, numbers, booleans, `null`, and `undefined`.

```javascript
let name = "Rob"; // String
let age = 25; // Number
let isDeveloper = true; // Boolean
let location = null; // Null
let description; // Undefined

```

* **Basic Operators:**
  * Arithmetic operators (`+`, `-`, `*`, `/`), assignment (`=`), comparison (`==`, `===`, `>`, `<`), and logical (`&&`, `||`).

```javascript
let sum = 10 + 5; // 15
let isEqual = (10 == '10'); // true with double equals
let isIdentical = (10 === '10'); // false with triple equals

```

* **Simple Functions:**
  * Function declarations vs. expressions, and introduction to arrow functions.

```javascript
// Function declaration
function greet(name) {
  return `Hello, ${name}!`;
}

// Arrow function
const greetArrow = name => `Hello, ${name}!`;
```

**Activities**

* Writing a function to greet a user
* Convert temperatures between Celsius and Fahrenheit.
* Count vowels in a given string.
