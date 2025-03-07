# Learn-javascript-with-me

### Table of Contents

<!-- TOC_START -->

| No. | Questions                                                                        |
| --- | -------------------------------------------------------------------------------- |
| 1   | [What is JavaScript?](#1-what-is-javascript)                                     |
| 2   | [Why Study JavaScript?](#2-why-study-javascript)                                 |
| 3   | [JavaScript Variables](#3-javascript-variables)                                  |
| 4   | [var/let/const](#4-varletconst)                                                  |
| 5   | [Difference Between var, let and const](#5-difference-between-var-let-and-const) |
| 6   | [JavaScript Data Types](#6-javascript-data-types)                                |

<!-- TOC_END -->

<!-- QUESTIONS_START -->

## 1. What is JavaScript

- JavaScript is the programming language of the web.
- It can update and change both HTML and CSS.
- It can calculate, manipulate and validate data.

**Note:**

- The Original JavaScript ES1 ES2 ES3 (1997-1999)
- The First Main Revision ES5 (2009)
- The Second Revision ES6 (2015)
- The Yearly Additions (2016, 2017 ... 2021, 2022)

## 2. Why Study JavaScript

- HTML to define the content of web pages.
- CSS to specify the layout of web pages.
- JavaScript to program the behavior of web pages.

## 3. JavaScript Variables

Variables in JavaScript can be declared using var, let, or const. JavaScript is dynamically typed, so variable types are determined at runtime without explicit type definitions.

**JavaScript Variables can be declared in 4 ways:**

- Automatically
- Using var
- Using let
- Using const

## 4. var/let/const

**var**

- var is a keyword in JavaScript used to declare variables and it is Function-scoped and hoisted, allowing redeclaration but can lead to unexpected bugs

```
function myFunction() {
  var message = "Hello World!"; // 'message' is only accessible within the 'myFunction' because it's declared with 'var'
  console.log(message);
}
myFunction(); // This will print "Hello World!"
console.log(message); // This will throw an error as 'message' is not accessible outside the function
```

**let**

- let is a keyword in JavaScript used to declare variables and it is Block-scoped and not hoisted to the top, suitable for mutable variables

```
let a = 12
let b = "gfg";
console.log(a);
console.log(b);

```

**const**

- const is a keyword in JavaScript used to declare variables and it is Block-scoped, immutable bindings that can’t be reassigned, though objects can still be mutated.

```
const a = 5
let b = "gfg";
console.log(a);
console.log(b);
```

## 5. Difference Between var, let and const

| Variable | Scope | Redeclare | Reassign | Hoisted |
| -------- | ----- | --------- | -------- | ------- |
| var      | No    | Yes       | Yes      | Yes     |
| let      | Yes   | No        | Yes      | No      |
| const    | Yes   | No        | No       | No      |

## 6. JavaScript Data Types

**JavaScript has 8 Datatypes**

- String
- Number
- Bigint
- Boolean
- Undefined
- Null
- Symbol
- Object

**The Object Datatype:**
The object data type can contain both built-in objects, and user defined objects:

Built-in object types can be:

objects, arrays, dates, maps, sets, intarrays, floatarrays, promises, and more.

```
// Numbers:
let length = 16;
let weight = 7.5;

// Strings:
let color = "Yellow";
let lastName = "Johnson";

// Booleans
let x = true;
let y = false;

// Object:
const person = {firstName:"John", lastName:"Doe"};

// Array object:
const cars = ["Saab", "Volvo", "BMW"];

// Date object:
const date = new Date("2022-03-25");

```

**Note:**
 - A JavaScript variable can hold any type of data.
 - JavaScript has dynamic types. This means that the same variable can be used to hold different data types:
```
let x;       // Now x is undefined
x = 5;       // Now x is a Number
x = "John";  // Now x is a String
```
- A string (or a text string) is a series of characters like "Rishabh Kashyap".

Strings are written with quotes. You can use single or double quotes.

- All JavaScript numbers are stored as decimal numbers (floating point).

Numbers can be written with, or without decimals.

<!-- ### Learn-javascript-with-me

Learn-javascript-with-me

- **Learn-javascript-with-me**
- Learn-javascript-with-me
  - Learn-javascript-with-me
    - Learn-javascript-with-me

1. Learn-javascript-with-me
2. Learn-javascript-with-me

```
console.log("Hello")
```

---

## 2. What is a prototype chain

## 3. my name is rishabh -->
