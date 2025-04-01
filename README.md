# Learn-javascript-with-me

### Table of Contents

<!-- TOC_START -->

| No. | Questions                                                                                                        |
| --- | ---------------------------------------------------------------------------------------------------------------- |
| 1   | [What is JavaScript?](#1-what-is-javascript)                                                                     |
| 2   | [Why Study JavaScript?](#2-why-study-javascript)                                                                 |
| 3   | [JavaScript Variables](#3-javascript-variables)                                                                  |
| 4   | [var/let/const](#4-varletconst)                                                                                  |
| 5   | [Difference Between var, let and const](#5-difference-between-var-let-and-const)                                 |
| 6   | [JavaScript Data Types](#6-javascript-data-types)                                                                |
| 7   | [What is String](#7-what-is-string)                                                                              |
| 8   | [What is Array](#8-what-is-array)                                                                                |
| 9   | [What is forEach](#9-what-is-foreach)                                                                            |
| 10  | [ Differences Between `forEach()` and Other Loops](#10-differences-between-foreach-and-other-loops)              |
| 11  | [ What is Map in JavaScript](#11-what-is-map-in-javascript)                                                      |
| 12  | [What is the filter Function](#12-what-is-the-filter-function)                                                   |
| 13  | [ Difference between filter , map , foreach](#13-difference-between-filter--map--foreach)                        |
| 14  | [ What is the reduce Function](#14-what-is-the-reduce-function)                                                  |
| 15  | [Difference Between `reduce()` vs `map()` vs `filter()`](#15-difference-between-reduce-vs-map-vs-filter)         |
| 16  | [What is an Object in JavaScript](#16-what-is-an-object-in-javascript)                                           |
| 17  | [for...in Loop / for...of Loop / Array.from() in js](#17-forin-loop--forof-loop--arrayfrom-in-js)                |
| 18  | [ Type Conversion vs Type Coercion](#18-type-conversion-vs-type-coercion)                                        |
| 19  | [What are Loops in JavaScript](#19-what-are-loops-in-javascript)                                                 |
| 20  | [What is a Function in JavaScript](#20-what-is-a-function-in-javascript)                                         |
| 21  | [Scope in JavaScript](#21-scope-in-javascript)                                                                   |
| 22  | [ Hoisting in JavaScript](#22-hoisting-in-javascript)                                                            |
| 23  | [Closures in JavaScript](#23closures-in-javascript)                                                              |
| 24  | [Callback Functions in JavaScript ](#24-callback-functions-in-javascript)                                        |
| 25  | [Higher-Order Functions](#25-higher-order-functions)                                                             |
| 26  | [Object and Array Destructuring in JavaScript](#26-object-and-array-destructuring-in-javascript)                 |
| 27  | [Array Methods: find(), some(), and every() ](#27-array-methods-find-some-and-every)                             |
| 28  | [Asynchronous JavaScript setTimeout setInterval](#28-asynchronous-javascript-settimeout-setinterval)             |
| 29  | [Event Loop in JavaScript](#29-event-loop-in-javascript)                                                         |
| 30  | [Spread and Rest Operators in JavaScript](#30-spread-and-rest-operators-in-javascript)                           |
| 31  | [ES6+ Features in JavaScript](#31-es6-features-in-javascript)                                                    |
| 32  | [Error Handling in JavaScript](#32-error-handling-in-javascript)                                                 |
| 33  | [Promises in JavaScript ](#33-promises-in-javascript)                                                            |
| 34  | [Async/Await in JavaScript](#34-asyncawait-in-javascript)                                                        |
| 35  | [Difference between async/await and .then() in promises](#35-difference-between-asyncawait-and-then-in-promises) |

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

[🔝 Back to Top](#table-of-contents)

## 2. Why Study JavaScript

- HTML to define the content of web pages.
- CSS to specify the layout of web pages.
- JavaScript to program the behavior of web pages.

[🔝 Back to Top](#table-of-contents)

## 3. JavaScript Variables

Variables in JavaScript can be declared using var, let, or const. JavaScript is dynamically typed, so variable types are determined at runtime without explicit type definitions.

**JavaScript Variables can be declared in 4 ways:**

- Automatically
- Using var
- Using let
- Using const

[🔝 Back to Top](#table-of-contents)

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

[🔝 Back to Top](#table-of-contents)

## 5. Difference Between var, let and const

| Variable | Scope | Redeclare | Reassign | Hoisted |
| -------- | ----- | --------- | -------- | ------- |
| var      | No    | Yes       | Yes      | Yes     |
| let      | Yes   | No        | Yes      | No      |
| const    | Yes   | No        | No       | No      |

## Key Differences Between `var`, `let`, and `const`

| Feature            | `var`                  | `let`                       | `const`                     |
| ------------------ | ---------------------- | --------------------------- | --------------------------- |
| **Scope**          | Function-scoped        | Block-scoped                | Block-scoped                |
| **Hoisting**       | Hoisted as `undefined` | Hoisted but not initialized | Hoisted but not initialized |
| **Reassignment**   | ✅ Allowed             | ✅ Allowed                  | ❌ Not Allowed              |
| **Redeclaration**  | ✅ Allowed             | ❌ Not Allowed              | ❌ Not Allowed              |
| **Initialization** | Optional               | Optional                    | Mandatory                   |

[🔝 Back to Top](#table-of-contents)

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

```javascript
let x; // Now x is undefined
x = 5; // Now x is a Number
x = "John"; // Now x is a String
```

- A string (or a text string) is a series of characters like "Rishabh Kashyap".

Strings are written with quotes. You can use single or double quotes.

- All JavaScript numbers are stored as decimal numbers (floating point).

Numbers can be written with, or without decimals.

[🔝 Back to Top](#table-of-contents)

**What is Template Literal**

Template literals are string literals that allow embedded expressions (variables) into your code. They are enclosed by backticks (`) instead of single (‘) or double (“) quotes.

- It was introduced in ES6, which provides a more flexible and readable way to work with strings.

```javascript
let a = "GFG";
console.log(`hello ${a}`);
```

[🔝 Back to Top](#table-of-contents)

## 7. What is String

- A string (or a text string) is a series of characters like "Rishabh Kashyap".

Strings are written with quotes. You can use single or double quotes.

```javascript
const string1 = "A string primitive";
const string2 = "Also a string primitive";
```

**Character access**

```javascript
"cat".charAt(1); // gives value "a"
"cat"[1]; // gives value "a"
```

**String objects**

```javascript
const strPrim = "foo"; // A literal is a string primitive
const strPrim2 = String(1); // Coerced into the string primitive "1"
const strPrim3 = String(true); // Coerced into the string primitive "true"
const strObj = new String(strPrim); // String with new returns a string wrapper object.

console.log(typeof strPrim); // "string"
console.log(typeof strPrim2); // "string"
console.log(typeof strPrim3); // "string"
console.log(typeof strObj); // "object"
```

**Static Method**

- String.fromCharCode()
- String.fromCodePoint()
- String.raw()

**Instance methods**

- **String.at()**

The at() method of String values takes an integer value and returns a new String
This method allows for positive and negative integers. Negative integers count back from the last string character.

```javascript
const sentence = "The quick brown fox jumps over the lazy dog.";

let index = 5;

console.log(`An index of ${index} returns the character ${sentence.at(index)}`);
// Expected output: "An index of 5 returns the character u"

index = -4;

console.log(`An index of ${index} returns the character ${sentence.at(index)}`);
// Expected output: "An index of -4 returns the character d"
```

- **String.charAt()**

The charAt() method of String values returns a new string at the given index.

```javascript
const sentence = "The quick brown fox jumps over the lazy dog.";

const index = 4;

console.log(`The character at index ${index} is ${sentence.charAt(index)}`);
// Expected output: "The character at index 4 is q"
```

- **String.prototype.charCodeAt()**

The charCodeAt() method of String values returns an integer between 0 and 65535

```javascript
const index = 4;

console.log(
  `Character code ${sentence.charCodeAt(index)} is equal to ${sentence.charAt(
    index
  )}`
);
// Expected output: "Character code 113 is equal to q"
```

- **String.concat()**

The concat() method of String values concatenates the string arguments to this string and returns a new string.

```javascript
const str1 = "Hello";
const str2 = "World";

console.log(str1.concat(" ", str2));
// Expected output: "Hello World"

console.log(str2.concat(", ", str1));
// Expected output: "World, Hello"
```

- **String.endsWith()**

The endsWith() method of String values determines whether a string ends with the characters of this string, returning true or false as appropriate.

```javascript
const str1 = "Cats are the best!";

console.log(str1.endsWith("best!"));
// Expected output: true

console.log(str1.endsWith("best", 17));
// Expected output: true

const str2 = "Is this a question?";

console.log(str2.endsWith("question"));
// Expected output: false
```

- **String.includes()**

The includes() method of String values performs a case-sensitive search to determine whether a given string may be found within this string, returning true or false as appropriate.

```javascript
const sentence = "The quick brown fox jumps over the lazy dog.";

const word = "fox";

console.log(
  `The word "${word}" ${
    sentence.includes(word) ? "is" : "is not"
  } in the sentence`
);
```

- **String.indexOf()**

```javascript
const paragraph = "I think Ruth's dog is cuter than your dog!";

const searchTerm = "dog";
const indexOfFirst = paragraph.indexOf(searchTerm);

console.log(`The index of the first "${searchTerm}" is ${indexOfFirst}`);
// Expected output: "The index of the first "dog" is 15"

console.log(
  `The index of the second "${searchTerm}" is ${paragraph.indexOf(
    searchTerm,
    indexOfFirst + 1
  )}`
);
// Expected output: "The index of the second "dog" is 38"
```

- **String.lastIndexOf()**

```javascript
const paragraph = "I think Ruth's dog is cuter than your dog!";

const searchTerm = "dog";

console.log(
  `Index of the last ${searchTerm} is ${paragraph.lastIndexOf(searchTerm)}`
);
// Expected output: "Index of the last "dog" is 38"
```

- **String.localeCompare()**

```javascript
const a = "réservé"; // With accents, lowercase
const b = "RESERVE"; // No accents, uppercase

console.log(a.localeCompare(b));
// Expected output: 1
```

- **String.repeat()**

```javascript
const mood = "Happy! ";

console.log(`I feel ${mood.repeat(3)}`);
// Expected output: "I feel Happy! Happy! Happy! "
```

- **String.replace()**

The original string is left unchanged.

```javascript
const paragraph = "I think Ruth's dog is cuter than your dog!";

console.log(paragraph.replace("Ruth's", "my"));
// Expected output: "I think my dog is cuter than your dog!"
```

- **String.replaceAll()**

The replaceAll() method of String values returns a new string with all matches of a pattern replaced by a replacement.

```javascript
const paragraph = "I think Ruth's dog is cuter than your dog!";

console.log(paragraph.replaceAll("dog", "monkey"));
// Expected output: "I think Ruth's monkey is cuter than your monkey!"
```

- **String.slice()**

The slice() method of String values extracts a section of this string and returns it as a new string, without modifying the original string.

```javascript
const str = "The quick brown fox jumps over the lazy dog.";

console.log(str.slice(31));
// Expected output: "the lazy dog."

console.log(str.slice(4, 19));
// Expected output: "quick brown fox"

console.log(str.slice(-4));
// Expected output: "dog."

console.log(str.slice(-9, -5));
// Expected output: "lazy"
```

```javascript
const str1 = "The morning is upon us."; // The length of str1 is 23.
const str2 = str1.slice(1, 8);
const str3 = str1.slice(4, -2);
const str4 = str1.slice(12);
const str5 = str1.slice(30);
console.log(str2); // he morn
console.log(str3); // morning is upon u
console.log(str4); // is upon us.
console.log(str5); // ""
```

```javascript
const str = "The morning is upon us.";
str.slice(-3); // 'us.'
str.slice(-3, -1); // 'us'
str.slice(0, -1); // 'The morning is upon us'
str.slice(4, -1); // 'morning is upon us'
```

- **String.split()**

```javascript
const str = "The quick brown fox jumps over the lazy dog.";

const words = str.split(" ");
console.log(words[3]);
// Expected output: "fox"

const chars = str.split("");
console.log(chars[8]);
// Expected output: "k"
```

```javascript
const emptyString = "";

// string is empty and separator is non-empty
console.log(emptyString.split("a"));
// [""]

// string and separator are both empty strings
console.log(emptyString.split(emptyString));
// []
```

```javascript
const myString = "Hello World. How are you doing?";
const splits = myString.split(" ", 3);

console.log(splits); // [ "Hello", "World.", "How" ]
```

- **String.startsWith()**

```javascript
const str1 = "Saturday night plans";

console.log(str1.startsWith("Sat"));
// Expected output: true

console.log(str1.startsWith("Sat", 3));
// Expected output: false
```

- **String.substring()**

```javascript
const str = "Mozilla";

console.log(str.substring(1, 3));
// Expected output: "oz"

console.log(str.substring(2));
// Expected output: "zilla"
```

- **String.toLowerCase()**

The toLowerCase() method of String values returns this string converted to lower case.

```javascript
const sentence = "The quick brown fox jumps over the lazy dog.";

console.log(sentence.toLowerCase());
// Expected output: "the quick brown fox jumps over the lazy dog."
```

- **String.toUpperCase()**

The toUpperCase() method of String values returns this string converted to uppercase.

```javascript
const sentence = "The quick brown fox jumps over the lazy dog.";

console.log(sentence.toUpperCase());
// Expected output: "THE QUICK BROWN FOX JUMPS OVER THE LAZY DOG."
```

- **String.trim()**

The trim() method of String values removes whitespace from both ends of this string and returns a new string, without modifying the original string.

```javascript
const greeting = "   Hello world!   ";

console.log(greeting);
// Expected output: "   Hello world!   ";

console.log(greeting.trim());
// Expected output: "Hello world!";
```

- **String.trimEnd()**

```javascript
const greeting = "   Hello world!   ";

console.log(greeting);
// Expected output: "   Hello world!   ";

console.log(greeting.trimEnd());
// Expected output: "   Hello world!";
```

- **String.trimStart()**

```javascript
const greeting = "   Hello world!   ";

console.log(greeting);
// Expected output: "   Hello world!   ";

console.log(greeting.trimStart());
// Expected output: "Hello world!   ";
```

- **String.valueOf()**

```javascript
const stringObj = new String("foo");
console.log(stringObj.valueOf());
// Expected output: "foo"
```

---

[🔝 Back to Top](#table-of-contents)

## 8. What is Array

An array in JavaScript is a special data structure used to store multiple values in a single variable.

- Arrays can contain different data types (numbers, strings, objects, even other arrays).
- Arrays are zero-indexed, meaning the first element is at index 0.
- Arrays are dynamic, meaning their size can change.

```javascript
let fruits = ["Apple", "Banana", "Mango"]; // Array of strings
let numbers = [10, 20, 30, 40]; // Array of numbers
let mixed = ["Hello", 42, true]; // Mixed data types
console.log(fruits[0]); // Output: Apple
console.log(numbers.length); // Output: 4
```

### Accessing & Modifying Arrays

- Use indexing to access elements.
- Use length property to find array size.
- Modify elements using indexing.

```javascript
let arr = ["a", "b", "c"];
console.log(arr[1]); // Output: "b"

arr[1] = "z"; // Modify element
console.log(arr); // Output: ["a", "z", "c"]

console.log(arr.length); // Output: 3
```

### Array Methods

**1. Adding & Removing Elements**

| Method           | Description                       | Example                        |
| ---------------- | --------------------------------- | ------------------------------ |
| `push(value)`    | Adds element to the **end**       | `arr.push(4)` → `[1, 2, 3, 4]` |
| `pop()`          | Removes last element              | `arr.pop()` → `[1, 2]`         |
| `unshift(value)` | Adds element to the **beginning** | `arr.unshift(0)` → `[0, 1, 2]` |
| `shift()`        | Removes first element             | `arr.shift()` → `[2, 3]`       |

```javascript
let arr = [1, 2, 3];

arr.push(4); // [1, 2, 3, 4]
arr.pop(); // [1, 2, 3]
arr.unshift(0); // [0, 1, 2, 3]
arr.shift(); // [1, 2, 3]
```

**2. Searching in Arrays**

| Method               | Description                  | Example                              |
| -------------------- | ---------------------------- | ------------------------------------ |
| `indexOf(value)`     | Finds first occurrence index | `[10, 20, 30].indexOf(20)` → `1`     |
| `lastIndexOf(value)` | Finds last occurrence index  | `[10, 20, 10].lastIndexOf(10)` → `2` |
| `includes(value)`    | Checks if value exists       | `[1, 2, 3].includes(2)` → `true`     |

```javascript
let arr = [10, 20, 30, 20];

console.log(arr.indexOf(20)); // Output: 1
console.log(arr.lastIndexOf(20)); // Output: 3
console.log(arr.includes(40)); // Output: false
```

**3. Iterating Through Arrays**

| Method                      | Description                         | Example                              |
| --------------------------- | ----------------------------------- | ------------------------------------ |
| `forEach(callback)`         | Loops through array                 | `arr.forEach((x) => console.log(x))` |
| `map(callback)`             | Creates a new array                 | `arr.map(x => x * 2)`                |
| `filter(callback)`          | Filters elements based on condition | `arr.filter(x => x > 2)`             |
| `reduce(callback, initial)` | Reduces array to a single value     | `arr.reduce((a, b) => a + b, 0)`     |

```javascript
let arr = [1, 2, 3, 4];

// forEach - Iteration
arr.forEach((num) => console.log(num)); // 1, 2, 3, 4

// map - Returns new array
let doubled = arr.map((num) => num * 2);
console.log(doubled); // [2, 4, 6, 8]

// filter - Returns filtered array
let greaterThanTwo = arr.filter((num) => num > 2);
console.log(greaterThanTwo); // [3, 4]

// reduce - Returns single value (sum)
let sum = arr.reduce((total, num) => total + num, 0);
console.log(sum); // 10
```

**4. Modifying & Sorting Arrays**

| Method                                 | Description                | Example                                      |
| -------------------------------------- | -------------------------- | -------------------------------------------- |
| `concat(arr2)`                         | Combines arrays            | `[1, 2].concat([3, 4])` → `[1, 2, 3, 4]`     |
| `join(separator)`                      | Converts array to string   | `[1,2,3].join('-')` → `"1-2-3"`              |
| `reverse()`                            | Reverses array             | `[1,2,3].reverse()` → `[3,2,1]`              |
| `sort()`                               | Sorts array (Alphabetical) | `["c", "a", "b"].sort()` → `["a", "b", "c"]` |
| `splice(start, deleteCount, ...items)` | Removes/adds elements      | `arr.splice(1,1,"X")`                        |
| `slice(start, end)`                    | Extracts portion of array  | `[1,2,3,4].slice(1,3)` → `[2,3]`             |

```javascript
let arr = ["Banana", "Apple", "Mango"];

// Sorting (Alphabetical order)
arr.sort();
console.log(arr); // ["Apple", "Banana", "Mango"]

// Splice - Remove & Add
arr.splice(1, 1, "Orange"); // Removes 1 element at index 1 and adds "Orange"
console.log(arr); // ["Apple", "Orange", "Mango"]

// Slice - Extract elements
let slicedArr = arr.slice(0, 2); // Extracts elements from index 0 to 1 (excluding index 2)
console.log(slicedArr); // ["Apple", "Orange"]
```

**5. Advanced Concepts**

- `Array Destructuring (ES6)`

```javascript
let [a, b, c] = [10, 20, 30];
console.log(a, b, c); // Output: 10 20 30
```

- `Spread Operator (...)`

```javascript
let arr1 = [1, 2, 3];
let arr2 = [...arr1, 4, 5]; // Copy and extend
console.log(arr2); // [1, 2, 3, 4, 5]
```

- `Checking if an Array (Array.isArray())`

```javascript
console.log(Array.isArray([1, 2, 3])); // true
console.log(Array.isArray("Hello")); // false
```

[🔝 Back to Top](#table-of-contents)

## 9. What is forEach

**Array.forEach()**

- The forEach() method of Array instances executes a provided function once for each array element.

```
const array1 = ["a", "b", "c"];
array1.forEach((element) => console.log(element));
// Expected output: "a"
// Expected output: "b"
// Expected output: "c"
```

```
const items = [
  {
    description: 'Apple',
    quantity: 4,
    price: 10
  },
  { description: 'Butter', quantity: 2, price: 5},
  { description: 'Snacks', quantity: 3, price: 6}
];
let flag=0;
let newarr=items.forEach((e,i)=>{
    let sum=items[i].quantity*items[i].price;
    flag=flag+sum;
});
     console.log(`Total Price : ${flag}`);

<!-- Output : Total Price : 68 -->
```

- **Syntax**

  - forEach(callbackFn)
  - forEach(callbackFn, thisArg)
  - array.forEach(callback(currentValue, index, array), thisArg);

  [🔝 Back to Top](#table-of-contents)

## 10. Differences Between `forEach()` and Other Loops

| Feature            | `forEach()`      | `for` Loop        | `map()`          |
| ------------------ | ---------------- | ----------------- | ---------------- |
| **Return Value**   | `undefined`      | N/A               | New Array        |
| **Break/Continue** | ❌ (Not Allowed) | ✅ (Allowed)      | ❌ (Not Allowed) |
| **Use Case**       | Side Effects     | General Iteration | Transform Data   |

🔹` forEach()`: Elements par operation perform karta hai, kuch return nahi karta.

🔹 `map()`: Naya transformed array return karta hai.

[🔝 Back to Top](#table-of-contents)

## 11. What is Map in JavaScript

The map() function is a built-in array method in JavaScript used to create a new array by applying a function to each element of an existing array.

Does not modify the original array.
Returns a new array with transformed elements.
Used for data transformation (e.g., doubling numbers, formatting strings).

```

let numbers = [1, 2, 3, 4];

// Using map() to double each number
let doubled = numbers.map(num => num \* 2);

console.log(doubled); // Output: [2, 4, 6, 8]
console.log(numbers); // Original array remains unchanged: [1, 2, 3, 4]

```

```

let numbers = [10, 20, 30];

let mappedArray = numbers.map((num, index, arr) => {
return `Index ${index}: ${num * 2}`;
});

console.log(mappedArray);
// Output: ["Index 0: 20", "Index 1: 40", "Index 2: 60"]

```

```
const items = [
  {
    description: 'Apple',
    quantity: 4,
    price: 10
  },
  { description: 'Butter', quantity: 2, price: 5},
  { description: 'Snacks', quantity: 3, price: 6}
];

let newarr=items.map((e,i)=>{
    return items[i].quantity*items[i].price;
});
console.log(newarr);

<!-- Output: [ 40, 10, 18 ] -->
```

**`map()` vs `forEach()`**
| Feature | `map()` | `forEach()` |
|-----------------------------|---------------|-----------------------------|
| **Returns a new array?** | ✅ Yes | ❌ No |
| **Can modify original array?** | ❌ No | ✅ Yes |
| **Used for transformation?** | ✅ Yes | ❌ No (only for iteration) |

[🔝 Back to Top](#table-of-contents)

## 12. What is the filter Function

The filter() function is a built-in array method in JavaScript that creates a new array containing only the elements that satisfy a given condition.

- Does not modify the original array.
- Returns a new array with filtered elements.
- Used for removing unwanted data from an array.

**Syntax:**

array.filter(function(element, index, array) {

    return condition; // Only elements where condition is true will be included

});

```

let numbers = [1, 2, 3, 4, 5, 6];

// Filter even numbers
let evenNumbers = numbers.filter(num => num % 2 === 0);

console.log(evenNumbers); // Output: [2, 4, 6]

```

```

let numbers = [10, 20, 30, 40, 50];

// Filter numbers at even indexes
let filtered = numbers.filter((num, index) => index % 2 === 0);

console.log(filtered); // Output: [10, 30, 50]

```

```
const items = [
  {
    description: 'Apple',
    quantity: 4,
    price: 10
  },
  { description: 'Butter', quantity: 2, price: 5},
  { description: 'Snacks', quantity: 3, price: 6}
];
let filteredItems=items.filter((e,i)=>{
    return items[i].quantity>2;
})
console.log(items);
console.log(filteredItems);

<!-- Output : [
  { description: 'Apple', quantity: 4, price: 10 },
  { description: 'Snacks', quantity: 3, price: 6 }
] -->

```

[🔝 Back to Top](#table-of-contents)

## 13. Difference between filter , map , foreach

| Feature                     | `filter()`               | `map()`             | `forEach()`                   |
| --------------------------- | ------------------------ | ------------------- | ----------------------------- |
| **Purpose**                 | Returns a filtered array | Transforms elements | Just loops through elements   |
| **Returns a new array?**    | ✅ Yes                   | ✅ Yes              | ❌ No                         |
| **Changes original array?** | ❌ No                    | ❌ No               | ✅ Yes (if modified manually) |

[🔝 Back to Top](#table-of-contents)

## 14. What is the reduce Function

The reduce() function is a higher-order array method in JavaScript that reduces an array to a single value by applying a function to each element.

- Used for sum, product, concatenation, flattening arrays, and more.
- Takes an accumulator (a running total) and each element of the array.
- Can return a number, string, object, or even another array.

**Syntax:**

array.reduce(function(accumulator, currentValue, index, array) {

return newAccumulator;

}, initialValue);

**or**

array.reduce((acc, curr) => newAcc, initialValue);

```

let numbers = [1, 2, 3, 4, 5];

// Sum of all numbers
let sum = numbers.reduce((acc, num) => acc + num, 0);

console.log(sum); // Output: 15

```

```
const items = [
  {
    description: 'Apple',
    quantity: 4,
    price: 10
  },
  { description: 'Butter', quantity: 2, price: 5},
  { description: 'Snacks', quantity: 3, price: 6}
];

let newarr=items.map((e,i)=>{
    return items[i].quantity*items[i].price;
});

console.log(newarr);

let filteredItems=items.filter((e,i)=>{
    return e.quantity>2;
})
console.log(items);
console.log(filteredItems);


let reduceItems=newarr.reduce((acc,c,i)=>{
    return acc+c;
},0)
console.log(reduceItems);

<!-- Output: [ 40, 10, 18 ]
[
  { description: 'Apple', quantity: 4, price: 10 },
  { description: 'Butter', quantity: 2, price: 5 },
  { description: 'Snacks', quantity: 3, price: 6 }
]
[
  { description: 'Apple', quantity: 4, price: 10 },
  { description: 'Snacks', quantity: 3, price: 6 }
]
68
 -->
```

**How It Works Internally:**

| Step | `acc` (Accumulator) | `num` (Current Element) | Calculation |
| ---- | ------------------- | ----------------------- | ----------- |
| 1    | 0                   | 1                       | 0 + 1 = 1   |
| 2    | 1                   | 2                       | 1 + 2 = 3   |
| 3    | 3                   | 3                       | 3 + 3 = 6   |
| 4    | 6                   | 4                       | 6 + 4 = 10  |
| 5    | 10                  | 5                       | 10 + 5 = 15 |

[🔝 Back to Top](#table-of-contents)

## 15. Difference Between `reduce()` vs `map()` vs `filter()`

| Feature                  | `reduce()`                      | `map()`             | `filter()`                            |
| ------------------------ | ------------------------------- | ------------------- | ------------------------------------- |
| **Purpose**              | Reduces array to a single value | Transforms elements | Filters elements based on a condition |
| **Returns a new array?** | ❌ No (returns a single value)  | ✅ Yes              | ✅ Yes                                |
| **Common Use**           | Summing, counting, merging      | Modifying values    | Removing unwanted elements            |

[🔝 Back to Top](#table-of-contents)

## 16. What is an Object in JavaScript

An object in JavaScript is a collection of key-value pairs. It allows you to store multiple values in a single variable.

- Keys are also called properties.
- Values can be any data type (string, number, array, function, etc.).
- Objects are used to group related data and behavior together.

  **Example:**

```
let person = {
    name: "Rishabh",
    age: 20,
    isStudent: true
};

console.log(person.name); // Output: Rishabh

```

**1. Creating Objects in JavaScript**

- Object Literal (Most Common)
- Using new Object()
- Using a Constructor Function
- Using Object.create()

```
<!-- Object Literal (Most Common)  -->

let car = {
    brand: "Toyota",
    model: "Camry",
    year: 2022
};

<!-- Using new Object() -->

let car = new Object();
car.brand = "Toyota";
car.model = "Camry";
car.year = 2022;

```

**2. Accessing Object Properties**

- Dot Notation (.)
- Bracket Notation ([])

```
<!-- Using Dot Notation (.)  -->

let person = {
    name: "Rishabh",
    age: 20,
    isStudent: true
};
console.log(person.name); // Output: Rishabh
```

```
<!-- using  Bracket Notation ([]) -->

let person = {
    "Full name": "Rishabh",
    age: 20,
    isStudent: true
};
console.log(person["Full name"]); // Output: Rishabh

```

**Note:** ✅ Use bracket notation when:

- The property name has spaces or special characters.
- The property name is stored in a variable.

**3. Adding, Updating, and Deleting Properties**

- Adding a New Property

  - Example:

         ```
         let person = {
         name: "Rishabh",
         age: 20,
         isStudent: true
         };
         person.city = "Delhi";
         console.log(person);
         // Output: { name: "Rishabh", age: 20, isStudent: true, city: "Delhi" }

          ```

- Updating a Property

  - Example:

    ```
    let person = {
    name: "Rishabh",
    age: 20,
    isStudent: true
    };
    person.age = 24;
    console.log(person.age); // Output: 24
    ```

- Deleting a Property

  - Example:

    ```
    let person = {
    name: "Rishabh",
    age: 20,
    isStudent: true
    };
    delete person.isStudent;
    console.log(person);
    // Output: { name: "Rishabh", age: 24
    }
    ```

**4. Looping Through an Object**

- Using for...in Loop
- Using Object.keys(), Object.values(), and Object.entries()

```

<!-- Using for...in Loop -->
 let person = {
    name: "Rishabh",
    age: 20,
    isStudent: true
    };

for (let key in person) {
    console.log(key, ":", person[key]);
}
/*
Output:
name : Rishabh
age : 20
   isStudent: true
*/
```

```
<!-- Using Object.keys(), Object.values(), and Object.entries() -->
 let person = {
    name: "Rishabh",
    age: 24,
    city: "Delhi"

    };

console.log(Object.keys(person));   // Output: ["name", "age", "city"]
console.log(Object.values(person)); // Output: ["Rishabh", 24, "Delhi"]
console.log(Object.entries(person)); // Output: [["name", "Rishabh"], ["age", 24], ["city", "Delhi"]]
```

**5. Object Methods (Functions Inside Objects)**

```
let person = {
    name: "Rishabh",
    age: 23,
    greet: function() {
        return `Hello, my name is ${this.name}`;
    }
};

console.log(person.greet()); // Output: Hello, my name is Rishabh
```

**Note: 📝 this refers to the current object.**

**6. Checking if a Property Exists**

```
let person = {
    name: "Rishabh",
    age: 24,
    city: "Delhi"

    };
console.log("age" in person); // Output: true
console.log(person.hasOwnProperty("city")); // Output: true
```

**7. Merging Objects**

- Using Object.assign()
- Using Spread Operator (...)

```
<!--Using Object.assign()  -->

let obj1 = { a: 1, b: 2 };
let obj2 = { b: 3, c: 4 };

let merged = Object.assign({}, obj1, obj2);
console.log(merged); // Output: { a: 1, b: 3, c: 4 }

```

```
<!-- Using Spread Operator (...) -->

let obj1 = { a: 1, b: 2 };
let obj2 = { b: 3, c: 4 };

let merged = { ...obj1, ...obj2 };
console.log(merged); // Output: { a: 1, b: 3, c: 4 }
```

**8. Objects vs Arrays**

| Feature       | Objects                            | Arrays                          |
| ------------- | ---------------------------------- | ------------------------------- |
| **Data Type** | Unordered key-value pairs          | Ordered list of elements        |
| **Access**    | By property name                   | By index number                 |
| **Best for**  | Storing structured data            | Storing lists of items          |
| **Methods**   | `Object.keys()`, `Object.values()` | `map()`, `filter()`, `reduce()` |

[🔝 Back to Top](#table-of-contents)

## 17. for...in Loop / for...of Loop / Array.from() in js

**1.for...in**

The for...in loop is used to iterate over the properties (keys) of an object.

```
let person = {
   name: "Rishabh",
   age: 23,
   city: "Delhi"
};

for (let key in person) {
   console.log(key, ":", person[key]);
}
/*
Output:
name : Rishabh
age : 23
city : Delhi
*/

```

**Example with an Array:**

```
let numbers = [10, 20, 30];

for (let index in numbers) {
    console.log(index, ":", numbers[index]);
}
/*
Output:
0 : 10
1 : 20
2 : 30
*/

```

**Note: for...in should not be used for arrays, because it iterates over indexes as strings, which can lead to unexpected results.**

**2. for...of**

The for...of loop is used to iterate over values of iterable objects like arrays, strings, sets, and maps.

```
let numbers = [10, 20, 30];

for (let num of numbers) {
   console.log(num);
}
/*
Output:
10
20
30
*/

```

**Example with a String:**

```
let name = "Rishabh";

for (let char of name) {
    console.log(char);
}
/*
Output:
R
i
s
h
a
b
h
*/
```

**3. Array.from()**

Array.from() is used to convert an iterable or array-like object into an array.

**Example 1: Convert a String to an Array**

```
let name = "Rishabh";
let charArray = Array.from(name);

console.log(charArray);
// Output: ['R', 'i', 's', 'h', 'a', 'b', 'h']

```

**Example 2: Convert arguments Object to an Array**

```
function sumAll() {
    let argsArray = Array.from(arguments);
    console.log(argsArray);
}

sumAll(5, 10, 15, 20);
// Output: [5, 10, 15, 20]
```

**Difference Between for...in and for...of**

## Difference Between `for...in` and `for...of`

| Feature                     | `for...in`                  | `for...of`                 |
| --------------------------- | --------------------------- | -------------------------- |
| **Iterates over**           | Object properties (keys)    | Values of iterable objects |
| **Works with Objects?**     | ✅ Yes                      | ❌ No                      |
| **Works with Arrays?**      | ✅ Yes, but not recommended | ✅ Yes                     |
| **Output for `{a:1, b:2}`** | `"a", "b"`                  | ❌ Error                   |
| **Output for `[1,2,3]`**    | `"0", "1", "2"`             | `1, 2, 3`                  |

```

let arr = [10, 20, 30];

for (let i in arr) {
    console.log(i); // Outputs: "0", "1", "2" (Indexes as Strings)
}

for (let value of arr) {
    console.log(value); // Outputs: 10, 20, 30
}


```

[🔝 Back to Top](#table-of-contents)

## 18. Type Conversion vs Type Coercion

| Feature        | Type Conversion                                                                                                           | Type Coercion                                                                            |
| -------------- | ------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| **Definition** | When we **explicitly** convert a data type into another type using methods like `Number()`, `String()`, `Boolean()`, etc. | When JavaScript **automatically** converts one data type into another during operations. |
| **Control**    | Done manually by the developer.                                                                                           | Done automatically by JavaScript.                                                        |
| **Example**    | `Number("10") → 10`                                                                                                       | `"5" * 2 → 10`                                                                           |

** 1. Type Conversion (Explicit)**

`✅ Converting to Number`

Use the Number() function to convert values to a number.

```
console.log(Number("10"));   // 10
console.log(Number("10.5")); // 10.5
console.log(Number("ABC"));  // NaN (Not a Number)
console.log(Number(true));   // 1
console.log(Number(false));  // 0
```

**Note:📌 Shortcut: parseInt() and parseFloat()**

```
console.log(parseInt("10.99"));  // 10
console.log(parseFloat("10.99")); // 10.99
```

`✅ Converting to String`

Use the String() function or .toString()

```
console.log(String(100));    // "100"
console.log(String(true));   // "true"
console.log((123).toString()); // "123"

```

`✅ Converting to Boolean`

Use Boolean() to convert values to true or false.

```
console.log(Boolean(1));    // true
console.log(Boolean(0));    // false
console.log(Boolean("Hello")); // true
console.log(Boolean(""));   // false
console.log(Boolean(null)); // false
console.log(Boolean(undefined)); // false

```

\*\*Note:`📝 Truthy Values: Any non-empty string, non-zero number, true.`

`📝 Falsy Values: 0, "", null, undefined, NaN, false.`\*\*

**2. Type Coercion (Implicit Conversion)**

JavaScript automatically converts data types in certain operations.

`✅ String Coercion (Number → String)`

```console.log("5" + 2);    // "52" (Number converted to String)
console.log("5" + true); // "5true" (Boolean converted to String)
console.log("5" + null); // "5null"
```

**Note:Addition (+) converts everything to a string!**

`✅ Number Coercion (String → Number)`

```
console.log("5" - 2);  // 3
console.log("5" * 2);  // 10
console.log("10" / "2"); // 5
console.log("10" - "5" + 2); // 7
console.log("10" - "5" + "2"); // "52" (String Concatenation)
```

**Note:📌 Subtraction (-), Multiplication (\*), and Division (/) convert strings to numbers automatically.**

`✅ Boolean Coercion (Convert to true or false)`

```
console.log(5 == "5");  // true (String converted to Number)
console.log(0 == false); // true (Boolean converted to Number)
console.log("" == false); // true
console.log(null == undefined); // true
```

**Note:📌 Loose equality (==) allows coercion, while strict equality (===) does not.**

`Equality Comparison (== vs ===)`

Loose Equality (`==`) vs Strict Equality (`===`)

| Operator | Meaning                          | Example             |
| -------- | -------------------------------- | ------------------- |
| `==`     | Loose equality (allows coercion) | `"5" == 5 → true`   |
| `===`    | Strict equality (no coercion)    | `"5" === 5 → false` |

✅ **Always prefer `===` to avoid unintended type conversions.**

```
console.log(5 == "5");  // true (Type coercion happens)
console.log(5 === "5"); // false (No coercion, types must match)

```

[🔝 Back to Top](#table-of-contents)

## 19. What are Loops in JavaScript

Loops are used to execute a block of code multiple times until a certain condition is met.

- `Types of Loops in JavaScript:`

1. for loop
2. while loop
3. do...while loop
4. for...in loop (for objects)
5. for...of loop (for iterables)

`1. for Loop (Entry-Controlled Loop)`

Used when we know how many times to run the loop.

- **Syntax**

```
for (initialization; condition; increment/decrement) {
   // Code to be executed
}

```

- **Example:**

```
for (let i = 1; i <= 5; i++) {
    console.log(i);
}
/*
Output:
1
2
3
4
5
*/

```

- **Example: Loop through an array**

```

let arr = [10, 20, 30, 40];

for (let i = 0; i < arr.length; i++) {
    console.log(arr[i]);
}
/*
Output:
10
20
30
40
*/

```

`2. while Loop (Entry-Controlled Loop)`

Used when we don’t know the exact number of iterations in advance.

- **Syntax**

```
while (condition) {
   // Code to be executed
}
```

- **Example:**

```

let i = 1;
while (i <= 5) {
console.log(i);
i++;
}
/_
Output:
1
2
3
4
5
_/

```

`3. do...while Loop (Exit-Controlled Loop)`

Executes at least once, even if the condition is false.

- **Syntax**

```
do {
   // Code to be executed
} while (condition);


```

- **Example:**

```
let i = 1;
do {
    console.log(i);
    i++;
} while (i <= 5);
/*
Output:
1
2
3
4
5
*/

```

- **Example: When Condition is Initially False**

```
let x = 10;
do {
    console.log("This will run once even if condition is false");
} while (x < 5);
/*
Output:
This will run once even if condition is false
*/

```

` 4. break and continue in Loops`

**✅ break Statement → Exits the loop immediately.**

```
for (let i = 1; i <= 5; i++) {
    if (i === 3) {
        break;
    }
    console.log(i);
}
/*
Output:
1
2
*/

```

**✅ continue Statement → Skips the current iteration and moves to the next.**

```
for (let i = 1; i <= 5; i++) {
    if (i === 3) {
        continue;
    }
    console.log(i);
}
/*
Output:
1
2
4
5
*/

```

`5. Nested Loops`

**✅ A loop inside another loop.**

```
for (let i = 1; i <= 3; i++) {
    for (let j = 1; j <= 3; j++) {
        console.log(`i = ${i}, j = ${j}`);
    }
}

<!-- output -->
<!--
i = 1, j = 1
i = 1, j = 2
i = 1, j = 3
i = 2, j = 1 -->


```

[🔝 Back to Top](#table-of-contents)

## 20. What is a Function in JavaScript

- A function is a block of reusable code that performs a specific task.
- It helps in code reusability, modularity, and better readability.

`Why Use Functions ?`

- ✅ Avoids code repetition
- ✅ Makes code modular and readable
- ✅ Helps in debugging and maintaining code

**1. Function Declaration (Named Function)**

- ✅ A function is defined using the function keyword.

- Syntax :

```
function functionName(parameters) {
    // Function body
    return value; // (Optional)
}
```

- **Example: Function to Add Two Numbers**

```
function add(a, b) {
    return a + b;
}

console.log(add(5, 3)); // Output: 8

```

` 📌 return keyword is used to send back the result. If no return, the function returns undefined.`

**2. Function Expression (Anonymous Function)**

- ✅ A function can be assigned to a variable.
- ✅ It does not have a name.

```
const subtract = function(a, b) {
    return a - b;
};

console.log(subtract(10, 5)); // Output: 5
```

`📌 Function expressions are not hoisted, so they cannot be called before declaration.`

**3. Arrow Functions (ES6)**

- ✅ A shorter way to write functions.
- ✅ Does not have its own `this`.

- `Syntax :`

```javascript
const functionName = (parameters) => expression;
```

- `Example : Arrow Function`

```javascript
const multiply = (a, b) => a * b;
console.log(multiply(4, 5)); // Output: 20
```

- `📌 If only one parameter, parentheses can be omitted :`

```javascript
const square = (x) => x * x;
console.log(square(4)); // Output: 16
```

- `📌 If function has multiple lines, use {} and return:`

```javascript
const greet = (name) => {
  return `Hello, ${name}`;
};
console.log(greet("Rishabh")); // Output: Hello, Rishabh
```

**4. Function Parameters & Default Parameters**

- ✅ Default parameters allow functions to have default values if no argument is passed.

```javascript
function greet(name = "Guest") {
  return `Hello, ${name}`;
}

console.log(greet("Rishabh")); // Output: Hello, Rishabh
console.log(greet()); // Output: Hello, Guest
```

**5. Rest Parameters (...args)**

- ✅ Allows functions to accept multiple arguments as an array.

```javascript
function sum(...numbers) {
  return numbers.reduce((acc, num) => acc + num, 0);
}

console.log(sum(1, 2, 3, 4, 5)); // Output: 15
```

`📌 Rest parameters must be the last parameter in the function.`

**6. Callback Functions**

- ✅ A function that is passed as an argument to another function.

```javascript
function greet(name, callback) {
  console.log(`Hello, ${name}`);
  callback();
}

function sayBye() {
  console.log("Goodbye!");
}

greet("Rishabh", sayBye);
/*
Output:
Hello, Rishabh
Goodbye!
*/
```

**7. Immediately Invoked Function Expression (IIFE)**

- ✅ A function that runs immediately after it is defined.
- ✅ Used to avoid polluting the global scope.

```javascript
(function () {
  console.log("IIFE is executed!");
})();
```

- `📌 With Arrow Function:`

```javascript
(() => console.log("IIFE with Arrow Function!"))();
```

**8. Higher-Order Functions**

- Takes another function as an argument.
- Returns another function as its result.

```javascript
function fun() {
  console.log("Hello, World!");
}
function fun2(action) {
  action();
  action();
}

fun2(fun);
```

[🔝 Back to Top](#table-of-contents)

## 21. Scope in JavaScript

- Scope in JavaScript refers to the accessibility and visibility of variables in different parts of the code.

**Types of Scope in JavaScript**

`1. Global Scope`

- A variable declared outside any function is in the global scope and can be accessed anywhere in the program.

```javascript
let globalVar = "I am global";

function showGlobal() {
  console.log(globalVar); // Accessible
}

showGlobal();
console.log(globalVar); // Accessible
```

- 🔹 Global variables can be accessed inside functions.
- 🔹 They remain in memory throughout the program execution.

`2. Local Scope (Function Scope)`

- A variable declared inside a function is in the local scope and cannot be accessed outside the function.

```javascript
function showLocal() {
  let localVar = "I am local";
  console.log(localVar); // Accessible inside function
}

showLocal();
console.log(localVar); // ❌ Error: localVar is not defined
```

- 🔹 Local variables are created when the function is called and destroyed when it ends.
- 🔹 They cannot be accessed outside the function.

`3. Block Scope (with let & const)`

- A block {} in JavaScript defines a block scope. Variables declared inside it using let or const cannot be accessed outside.

```javascript
{
  let blockVar = "I am block-scoped";
  console.log(blockVar); // Accessible inside block
}

console.log(blockVar); // ❌ Error: blockVar is not defined
```

- let and const are block-scoped, but var is not!

`Example: var is NOT block-scoped`

```javascript
{
  var test = "I am NOT block-scoped";
}
console.log(test); // ✅ Accessible
```

`4.  Lexical Scope (Nested Scope)`

- In JavaScript, inner functions can access variables from their parent functions. This is called lexical scope.

```javascript
function outer() {
  let outerVar = "I am from outer function";

  function inner() {
    console.log(outerVar); // ✅ Accessible
  }

  inner();
}

outer();
```

- 🔹 Inner functions inherit variables from their parent functions, but the reverse is not true.

`5. Closures (Advanced Concept)`

- A closure is a function that remembers the variables from its lexical scope even after the outer function has finished executing.

```javascript
function init() {
  var name = "Mozilla"; // name is a local variable created by init
  function displayName() {
    // displayName() is the inner function, that forms a closure
    console.log(name); // use variable declared in the parent function
  }
  displayName();
}
init();
```

[🔝 Back to Top](#table-of-contents)

## 22. Hoisting in JavaScript

- Hoisting is JavaScript’s default behavior of moving declarations to the top of their scope before execution. This means you can use variables and functions before declaring them.

**1. How Hoisting Works**

```javascript
console.log(a); // ❌ Undefined (Not an error, but variable is not assigned yet)
var a = 10;
console.log(a); // ✅ 10
```

- 🔹 JavaScript moves the declaration (var a;) to the top but not the initialization (a = 10;).
- 🔹 This is why the first console.log(a) prints undefined instead of an error.

**2. Hoisting with var, let, and const**

`
`var`vs`let`vs`const` (Hoisting & Initialization)

| Keyword | Hoisted? | Initialized with Default Value? | Can be Accessed Before Declaration? |
| ------- | -------- | ------------------------------- | ----------------------------------- |
| `var`   | ✅ Yes   | `undefined`                     | ✅ Yes (but returns `undefined`)    |
| `let`   | ✅ Yes   | ❌ No (Temporal Dead Zone)      | ❌ No (Reference Error)             |
| `const` | ✅ Yes   | ❌ No (Temporal Dead Zone)      | ❌ No (Reference Error)             |

`✅ Example with var`

```javascript
console.log(x); // ❌ Undefined (Variable exists but is not assigned)
var x = 5;
console.log(x); // ✅ 5
```

`✅ Example with let`

```javascript
console.log(y); // ❌ ReferenceError (Cannot access 'y' before initialization)
let y = 5;
console.log(y); // ✅ 5
```

- 🔹 let is hoisted but stays in the "Temporal Dead Zone" (TDZ) until it is initialized.

`✅ Example with const`

```javascript
console.log(z); // ❌ ReferenceError (Cannot access 'z' before initialization)
const z = 5;
console.log(z); // ✅ 5
```

- 🔹 Like let, const is also in the "Temporal Dead Zone" and must be initialized at the time of declaration.

**3. Function Hoisting**

- Function declarations are completely hoisted, meaning you can call them before declaring.

```javascript
greet(); // ✅ Works fine

function greet() {
  console.log("Hello, Rishabh!");
}
```

- 🔹 The entire function is hoisted, so it works before declaration.

`❌ Function Expression Hoisting (Using var)`

```javascript
sayHello(); // ❌ TypeError: sayHello is not a function

var sayHello = function () {
  console.log("Hello!");
};
```

🔹 Only var sayHello is hoisted, but not the function assignment.
🔹 At the time of execution, sayHello is still undefined, causing an error.

`✅ Function Expression Hoisting (Using let or const)`

```javascript
greet(); // ❌ ReferenceError: Cannot access 'greet' before initialization

let greet = function () {
  console.log("Hello!");
};
```

🔹 let and const are hoisted but stay in the Temporal Dead Zone, so calling greet() before declaration causes an error.

[🔝 Back to Top](#table-of-contents)

## 23.Closures in JavaScript

A closure in JavaScript is a function that remembers the variables from its outer scope, even after the outer function has finished executing.

**1. Basic Example**

```javascript
function outer() {
  let count = 0; // Local variable in outer function

  function inner() {
    count++; // Inner function accesses outer function's variable
    console.log(count);
  }

  return inner; // Returning inner function
}

const counter = outer(); // outer() executes and returns inner()
counter(); // Output: 1
counter(); // Output: 2
counter(); // Output: 3
```

**2. Closures in Real-World Scenarios**

`✅ Use Case 1: Data Hiding (Encapsulation)`

- Closures allow us to create private variables in JavaScript.

```javascript
function createCounter() {
  let count = 0; // Private variable

  return {
    increment: function () {
      count++;
      console.log(count);
    },
    decrement: function () {
      count--;
      console.log(count);
    },
    getCount: function () {
      return count;
    },
  };
}

const counter = createCounter();
counter.increment(); // 1
counter.increment(); // 2
counter.decrement(); // 1
console.log(counter.getCount()); // 1
```

`✅ Use Case 2: Function Factory`

```javascript
function multiplier(factor) {
  return function (num) {
    return num * factor;
  };
}

const double = multiplier(2);
const triple = multiplier(3);

console.log(double(5)); // Output: 10
console.log(triple(5)); // Output: 15
```

- Each function (double and triple) keeps its own factor value due to closures.

`✅ Use Case 3: Delayed Execution (setTimeout & Closures)`

```javascript
function delayedGreeting(name, delay) {
  setTimeout(() => {
    console.log(`Hello, ${name}!`);
  }, delay);
}

delayedGreeting("Rishabh", 2000); // Output after 2 seconds: "Hello, Rishabh!"
```

`The callback inside setTimeout retains access to name, even after delayedGreeting has finished executing.`

[🔝 Back to Top](#table-of-contents)

## 24. Callback Functions in JavaScript

A callback function is a function that is passed as an argument to another function and is executed later.

1. `Basic Example of a Callback Function`

```javascript
function greet(name, callback) {
  console.log("Hello, " + name);
  callback(); // Executing the callback function
}

function sayGoodbye() {
  console.log("Goodbye!");
}

greet("Rishabh", sayGoodbye);
// Output:
// Hello, Rishabh
// Goodbye!
```

`✅ The sayGoodbye function is passed as a callback to greet() and gets executed inside greet()`

2. `Why Use Callback Functions?`

- To execute a function after another function completes.
- To handle asynchronous operations (e.g., API calls, file reading, timers).
- To allow flexibility and reusability of functions.

3. `Callback with Anonymous Function`

- Instead of defining a separate function, we can pass an anonymous function directly.

```javascript
function greet(name, callback) {
  console.log("Hello, " + name);
  callback();
}

greet("Rishabh", function () {
  console.log("This is an anonymous callback function.");
});
```

- ✅ Shorter syntax without needing an extra function name.

4. `Callback in Asynchronous JavaScript (setTimeout)`

```javascript
console.log("Start");

setTimeout(function () {
  console.log("This message appears after 2 seconds");
}, 2000);

console.log("End");
```

- ✅ setTimeout() executes the callback after 2 seconds without blocking the code execution.

5. `Callback in Array Methods (forEach, map, filter)`

`✅ Using forEach()`

```javascript
let numbers = [1, 2, 3];

numbers.forEach(function (num) {
  console.log(num * 2);
});
// Output: 2, 4, 6
```

- ✅ The callback function modifies each element in the array.

`✅ Using map()`

```javascript
let doubled = numbers.map(function (num) {
  return num * 2;
});
console.log(doubled); // Output: [2, 4, 6]
```

6. `Callback Function in Event Handling`

```javascript
document.getElementById("btn").addEventListener("click", function () {
  console.log("Button clicked!");
});
```

- ✅ The callback function runs only when the button is clicked.

7. `Nested Callbacks (Callback Hell)`

- When using callbacks in asynchronous functions, nested callbacks can make the code hard to read and maintain.

```javascript
function step1(callback) {
  setTimeout(() => {
    console.log("Step 1 completed");
    callback();
  }, 1000);
}

function step2(callback) {
  setTimeout(() => {
    console.log("Step 2 completed");
    callback();
  }, 1000);
}

function step3() {
  setTimeout(() => {
    console.log("Step 3 completed");
  }, 1000);
}

// Callback hell (nested callbacks)
step1(() => {
  step2(() => {
    step3();
  });
});
```

- ❌ This is called "Callback Hell" because the code is deeply nested and hard to manage.

- ✅ Solution: Use Promises or Async/Await (we will learn later).

`NOTE`

Callbacks can be either synchronous or asynchronous, depending on the context in which they are called, not inherently one or the other. A callback is synchronous if the function that calls it executes the callback immediately, while an asynchronous callback is executed later, after an asynchronous operation completes

`Synchronous Callbacks:`

When a function immediately calls the callback after it has completed its task, it's a synchronous callback

`Asynchronous Callbacks:`

If the function that calls the callback uses asynchronous operations, such as network requests or timers, the callback is executed later, after the asynchronous operation completes

`Example :`

- **Synchronous** : myArray.forEach(callbackFunction) (the callback is executed immediately for each element).
- **Asynchronous** : setTimeout(callbackFunction, 1000) (the callback is executed after 1000 milliseconds

[🔝 Back to Top](#table-of-contents)

## 25. Higher-Order Functions

A Higher-Order Function (HOF) is a function that takes another function as an argument or returns a function as a result

- `Example`

```javascript
function greet(name) {
  return function (message) {
    console.log(`Hello ${name}, ${message}`);
  };
}

const greetRishabh = greet("Rishabh");
greetRishabh("Good Morning!"); // Output: Hello Rishabh, Good Morning!
```

- ✅ greet() returns another function, which remembers the name due to closures.

**1. Why Use Higher-Order Functions?**

- Code reusability
- Better readability & maintainability
- Useful for functional programming

**2. HOFs with Callbacks**

Higher-order functions take a function as an argument.

- `Example :`

```javascript
function operate(num1, num2, operation) {
  return operation(num1, num2);
}

function add(a, b) {
  return a + b;
}

function multiply(a, b) {
  return a * b;
}

console.log(operate(5, 3, add)); // Output: 8
console.log(operate(5, 3, multiply)); // Output: 15
```

- ✅ operate() is a Higher-Order Function because it takes operation (a function) as an argument.

**3. Common Higher-Order Functions in JavaScript**

- JavaScript provides several built-in HOFs like map(), filter(), reduce().

`✅ Using map()`

```javascript
let numbers = [1, 2, 3, 4];

let doubled = numbers.map(function (num) {
  return num * 2;
});

console.log(doubled); // Output: [2, 4, 6, 8]
```

`✅ map() is a HOF because it takes a function as an argument and applies it to each array element.`

`✅ Using filter()`

```javascript
let numbers = [1, 2, 3, 4];
let evenNumbers = numbers.filter(function (num) {
  return num % 2 === 0;
});

console.log(evenNumbers); // Output: [2, 4]
```

```
✅ filter() takes a function and filters elements based on a condition.

```

`✅ Using reduce()`

```javascript
let numbers = [1, 2, 3, 4];

let sum = numbers.reduce(function (total, num) {
  return total + num;
}, 0);

console.log(sum); // Output: 10
```

`✅ reduce() accumulates values based on the provided function.`

**4. HOF Returning a Function**

- Higher-order functions can return another function.

```javascript
function power(exponent) {
  return function (number) {
    return Math.pow(number, exponent);
  };
}

const square = power(2);
const cube = power(3);

console.log(square(5)); // Output: 25
console.log(cube(2)); // Output: 8
```

[🔝 Back to Top](#table-of-contents)

## 26. Object and Array Destructuring in JavaScript

Destructuring is a feature in JavaScript that allows you to unpack values from arrays or properties from objects easily into variables.

**1. Array Destructuring**

Instead of accessing elements one by one, we can use destructuring.

```javascript
const numbers = [10, 20, 30];

const [a, b, c] = numbers;

console.log(a); // Output: 10
console.log(b); // Output: 20
console.log(c); // Output: 30
```

`✅ Each variable gets a corresponding array element based on its position.`

**2. Skipping Values in Array Destructuring**

```javascript
const numbers = [10, 20, 30, 40];

const [first, , third] = numbers;

console.log(first); // Output: 10
console.log(third); // Output: 30
```

`✅ Skipping the second element (20) using , , notation.`

**3. Swapping Variables Using Destructuring**

- A simple way to swap two variables without using a third variable.

```javascript
let x = 5,
  y = 10;

[x, y] = [y, x];

console.log(x); // Output: 10
console.log(y); // Output: 5
```

`✅ Directly swaps values without using extra variables.`

**4. Rest Operator in Array Destructuring**

- You can use the rest operator (...) to collect remaining values.

```javascript
const numbers = [1, 2, 3, 4, 5];

const [first, second, ...rest] = numbers;

console.log(first); // Output: 1
console.log(second); // Output: 2
console.log(rest); // Output: [3, 4, 5]
```

`✅ The rest variable collects all remaining values into an array.`

**5. Object Destructuring**

Extract values from an object easily.

```javascript
const person = {
  name: "Rishabh",
  age: 22,
  city: "Delhi",
};

const { name, age, city } = person;

console.log(name); // Output: Rishabh
console.log(age); // Output: 22
console.log(city); // Output: Delhi
```

`✅ Each variable gets the value of the corresponding object property.`

**6. Renaming Variables While Destructuring**

- You can rename variables to avoid conflicts.

```javascript
const user = {
  username: "rishabh123",
  email: "rishabh@example.com",
};

const { username: userName, email: userEmail } = user;

console.log(userName); // Output: rishabh123
console.log(userEmail); // Output: rishabh@example.com
```

`✅ username is renamed as userName and email as userEmail.`

**7. Default Values in Object Destructuring**

- If a property doesn't exist, a default value is assigned.

```javascript
const person = { name: "Rishabh", age: 22 };

const { name, age, country = "India" } = person;

console.log(name); // Output: Rishabh
console.log(age); // Output: 22
console.log(country); // Output: India (default value)
```

`✅ If country is missing, the default value "India" is used.`

**8. Nested Object Destructuring**

- You can extract values from nested objects.

```javascript
const employee = {
  id: 101,
  details: {
    name: "Rishabh",
    department: "IT",
  },
};

const {
  details: { name, department },
} = employee;

console.log(name); // Output: Rishabh
console.log(department); // Output: IT
```

`✅ Extracting name and department from the details object.`

**9. Function Parameters with Destructuring**

`✅ Array Destructuring in Functions`

```javascript
function sum([a, b]) {
  return a + b;
}

console.log(sum([5, 10])); // Output: 15
```

✅ Function takes an array as an argument and destructures it inside the parameter list.

`✅ Object Destructuring in Functions`

```
function displayUser({ name, age }) {
    console.log(`User: ${name}, Age: ${age}`);
}

const user = { name: "Rishabh", age: 22, city: "Delhi" };

displayUser(user);
// Output: User: Rishabh, Age: 22
```

✅ Only name and age are extracted from the user object.

[🔝 Back to Top](#table-of-contents)

## 27. Array Methods: find(), some(), and every()

JavaScript provides powerful array methods like find(), some(), and every() to help search, validate, and check conditions efficiently.

**1. find() Method**

- The find() method returns the first element in an array that satisfies a condition.

```javascript
const numbers = [10, 25, 30, 45, 50];

const result = numbers.find((num) => num > 20);

console.log(result); // Output: 25 (first number greater than 20)
```

- find() stops searching once it finds the first match.

`✅ find() with Objects`

```javascript
const users = [
  { id: 1, name: "Rishabh", age: 22 },
  { id: 2, name: "Amit", age: 25 },
  { id: 3, name: "Raj", age: 30 },
];

const user = users.find((person) => person.age > 24);

console.log(user);
// Output: { id: 2, name: "Amit", age: 25 }
```

- ✅ find() returns the first object where age > 24.

`✅ When find() Returns undefined`

- If no match is found, find() returns undefined.

```javascript
const numbers = [1, 3, 5, 7];

const result = numbers.find((num) => num % 2 === 0);

console.log(result); // Output: undefined (no even number)
```

**2. some() Method**

- The some() method checks if at least one element in the array satisfies a condition. It returns true or false.

```javascript
const numbers = [1, 3, 5, 8];

const hasEven = numbers.some((num) => num % 2 === 0);

console.log(hasEven); // Output: true (because 8 is even)
```

- ✅ Returns true if any element passes the test.

`✅ some() with Objects`

```javascript
const users = [
  { name: "Rishabh", age: 22 },
  { name: "Amit", age: 17 },
  { name: "Raj", age: 30 },
];

const isAdultPresent = users.some((user) => user.age >= 18);

console.log(isAdultPresent); // Output: true (at least one person is 18+)
```

- Checks if any object has age >= 18.

`✅ When some() Returns false`

- If no match is found, it returns false.

```
const numbers = [1, 3, 5, 7];

const hasEven = numbers.some(num => num % 2 === 0);

console.log(hasEven); // Output: false (no even number)
```

**3. every() Method**

- The every() method checks if all elements satisfy a condition. It returns true or false.

```
const numbers = [2, 4, 6, 8];

const allEven = numbers.every(num => num % 2 === 0);

console.log(allEven); // Output: true (all are even)

```

- ✅ Returns true only if all elements pass the condition.

`✅ every() with Objects`

```
const users = [
    { name: "Rishabh", age: 22 },
    { name: "Amit", age: 18 },
    { name: "Raj", age: 30 }
];

const allAdults = users.every(user => user.age >= 18);

console.log(allAdults); // Output: true (all users are 18+)
```

✅ Checks if all users are adults (age >= 18).

`✅ When every() Returns false`

- If any element fails the condition, it returns false.

```
const numbers = [2, 4, 6, 7];

const allEven = numbers.every(num => num % 2 === 0);

console.log(allEven); // Output: false (because 7 is odd)
```

**Differences Between `find()`, `some()`, and `every()`**

| Method    | Returns                               | Stops Searching After | Used For                                    |
| --------- | ------------------------------------- | --------------------- | ------------------------------------------- |
| `find()`  | First matching element or `undefined` | First match           | Finding an element                          |
| `some()`  | `true` or `false`                     | First `true` value    | Checking if **at least one** element passes |
| `every()` | `true` or `false`                     | First `false` value   | Checking if **all** elements pass           |

### Key Points:

- **`find()`** returns the first matching element and stops searching.
- **`some()`** returns `true` if **at least one** element satisfies the condition.
- **`every()`** returns `true` only if **all** elements satisfy the condition.

[🔝 Back to Top](#table-of-contents)

## 28. Asynchronous JavaScript setTimeout setInterval

JavaScript is single-threaded, meaning it executes one task at a time. However, it can handle asynchronous operations using functions like setTimeout and setInterval. These functions allow JavaScript to perform delayed execution and repeated execution without blocking the main thread.

**1. What is Asynchronous JavaScript?**

🔹 `Synchronous JavaScript` → Executes line by line, blocking further execution.

🔹 `Asynchronous JavaScript` → Executes non-blocking operations like timers, API calls, and event listeners.

🔹 `Example of Synchronous vs Asynchronous`

```javascript
console.log("Start");

setTimeout(() => console.log("Inside setTimeout"), 2000);

console.log("End");
```

✅ Output:

```
Start
End
Inside setTimeout
```

🔹 JavaScript doesn’t wait for setTimeout(2000) to finish and executes "End" first.

**2. setTimeout() – Execute Code After Delay**

🔹 `setTimeout()` executes a function after a specified delay (in milliseconds).

🔹`Syntax:`

```javascript
setTimeout(function, delay, param1, param2, ...);
```

🔹`Example`:

```javascript
console.log("Before setTimeout");

setTimeout(() => {
  console.log("Executed after 2 seconds");
}, 2000);

console.log("After setTimeout");
```

`✅ Output:`

```javascript
Before setTimeout
After setTimeout
Executed after 2 seconds
```

🔹 The delay does not pause JavaScript execution.

**3. setTimeout with Parameters**

You can pass arguments to the callback function in setTimeout.

```javascript
function greet(name) {
  console.log(`Hello, ${name}!`);
}

setTimeout(greet, 3000, "Rishabh");
// Output after 3 seconds: Hello, Rishabh!
```

`Note: ✅ No need to use an anonymous function.`

**4. Clearing setTimeout (Stopping Execution)**

Use clearTimeout() to cancel a scheduled setTimeout.

```javascript
let timer = setTimeout(() => console.log("This will not run"), 3000);
clearTimeout(timer);
```

✅ The function inside setTimeout is never executed.

**5. setInterval() – Repeated Execution**

🔹 setInterval() executes a function repeatedly after a specified interval.

🔹`Syntax:`

```javascript
setInterval(function, interval, param1, param2, ...);
```

🔹`Example:`

```javascript
let count = 1;

let interval = setInterval(() => {
  console.log(`Count: ${count}`);
  count++;

  if (count > 5) clearInterval(interval);
}, 1000);
```

`✅ Output:`

```
Count: 1
Count: 2
Count: 3
Count: 4
Count: 5
```

🔹 clearInterval(interval) stops the repeated execution.

**6. Real-World Example: Digital Clock**

```javascript
setInterval(() => {
  let time = new Date().toLocaleTimeString();
  console.log(time);
}, 1000);
```

✅ Displays the current time every second.

**7. Difference Between `setTimeout` and `setInterval`**

| Feature       | `setTimeout()`            | `setInterval()`                    |
| ------------- | ------------------------- | ---------------------------------- |
| **Execution** | Runs **once** after delay | Runs **repeatedly** at intervals   |
| **Use Case**  | Delayed execution         | Continuous execution (like timers) |
| **Stopping**  | `clearTimeout()`          | `clearInterval()`                  |

**8. setTimeout Inside setTimeout (Recursive setTimeout)**

🔹 Instead of setInterval, you can use recursive setTimeout for better control.

```javascript
function repeat() {
  console.log("Hello!");
  setTimeout(repeat, 1000);
}

repeat();
```

✅ This approach is better because it avoids overlapping executions.

[🔝 Back to Top](#table-of-contents)

## 29. Event Loop in JavaScript

- In the world of JavaScript, the event loop is a mechanism that enables asynchronous operations to be executed in a non-blocking manner.

- JavaScript is single-threaded, it uses the event loop to manage the execution of multiple tasks without blocking the main thread.

- JavaScript is single-threaded, meaning it executes one operation at a time. However, it can handle asynchronous tasks like API calls, timers, and DOM events without blocking execution. This is managed by the Event Loop.

**2. JavaScript Execution Model**

JavaScript uses the following components to handle code execution:

- Call Stack – Executes synchronous code.

- Web APIs – Handles async tasks (e.g., setTimeout, fetch).

- Callback Queue – Stores callbacks for execution.

- Microtask Queue – Stores promises and MutationObserver tasks.

- Event Loop – Moves tasks from the queue to the call stack.

**3. How the Event Loop Works?**

Step-by-Step Process:

1️⃣ Synchronous code runs first (inside the Call Stack).

2️⃣ Asynchronous tasks (like setTimeout, fetch, Promises) move to Web APIs.

3️⃣ Once an async task is complete, its callback is placed in either:

- Microtask Queue (for Promises, MutationObserver).

- Callback Queue (for setTimeout, setInterval, DOM events).

4️⃣ Event Loop checks:

- If the Call Stack is empty, it moves tasks from the Microtask Queue first.

- Then, it moves tasks from the Callback Queue (if no microtasks are pending).

**4. Example: Understanding Event Loop**

Synchronous vs Asynchronous Execution

```javascript
console.log("Start");

setTimeout(() => console.log("Inside setTimeout"), 0);

Promise.resolve().then(() => console.log("Inside Promise"));

console.log("End");
```

**`Execution Order:`**

- 1️⃣ `"Start"` → (Synchronous, runs first in Call Stack)
- 2️⃣ `"End"` → (Synchronous, runs second in Call Stack)
- 3️⃣ `"Inside Promise"` → (Microtask Queue, runs before setTimeout)
- 4️⃣ `"Inside setTimeout"` → (Callback Queue, runs last)

**`Working`**

The event loop in JavaScript handles asynchronous tasks and ensures smooth execution. When the code runs, JavaScript first executes all synchronous tasks line by line.

- "Start" is logged first.

- The setTimeout() function is called, but since it is asynchronous, it goes to the Web APIs and waits for the timer to finish.

- The Promise is also asynchronous, but it gets added to the microtask queue (which has higher priority than the callback queue of setTimeout()).

- "End" is logged next because it's synchronous.

- The event loop checks the microtask queue first, so "Inside Promise" is logged.

- Finally, the event loop processes the callback queue, logging "Inside setTimeout".

**`output`**

```javascript
Start
End
Inside Promise
Inside setTimeout
```

**`Note:` 🔹 Promise executes before setTimeout because microtasks have higher priority.**

**5. Microtask vs. Callback Queue (Priority Order)**

| Task Type                                        | Execution Order                         |
| ------------------------------------------------ | --------------------------------------- |
| Synchronous Code                                 | Runs first in Call Stack                |
| Microtask Queue (Promises, MutationObserver)     | Runs immediately after synchronous code |
| Callback Queue (setTimeout, setInterval, Events) | Runs after Microtasks are cleared       |

**6. Example: Microtask Priority Over setTimeout**

```javascript
setTimeout(() => console.log("setTimeout"), 0);

Promise.resolve().then(() => console.log("Promise resolved"));

console.log("Sync Code");
```

**output**

```javascript
Sync Code
Promise resolved
setTimeout
```

`🔹 Promise resolves before setTimeout because Microtasks run first.`

**7. Real-World Use Cases of the Event Loop**

🔹 Handling API Calls Efficiently

```javascript
console.log("Fetching data...");

fetch("https://jsonplaceholder.typicode.com/todos/1")
  .then((response) => response.json())
  .then((data) => console.log("Data received:", data));

console.log("Waiting for response...");
```

`✅ JavaScript doesn’t wait for fetch() to complete and executes the next statement!`

[🔝 Back to Top](#table-of-contents)

## 30. Spread and Rest Operators in JavaScript

JavaScript introduced Spread (...) and Rest (...) operators in ES6. Though they look the same (...), they serve different purposes.

🔹 `Spread (...)` → Expands elements from arrays/objects.

🔹 `Rest (...)` → Gathers multiple elements into an array.

**1. Spread Operator (...) – Expanding Elements**

- `Expanding an Array`

```javascript
const arr1 = [1, 2, 3];
const arr2 = [...arr1, 4, 5, 6];

console.log(arr2);
// Output: [1, 2, 3, 4, 5, 6]
```

`✅ Spread operator expands elements from arr1 into arr2.`

- `Copying an Array (Avoids Reference Issues)`

```javascript
const original = [10, 20, 30];
const copy = [...original];

copy.push(40);

console.log(original); // [10, 20, 30] (Original remains unchanged)
console.log(copy); // [10, 20, 30, 40]
```

`✅ Unlike = assignment, the spread operator creates a new array, not a reference.`

- `Merging Arrays`

```javascript
const first = [1, 2];
const second = [3, 4];
const merged = [...first, ...second];

console.log(merged);
// Output: [1, 2, 3, 4]
```

`✅ Merges arrays without using concat().`

- `Using Spread in Function Arguments`

```javascript
function sum(a, b, c) {
  return a + b + c;
}

const numbers = [10, 20, 30];

console.log(sum(...numbers));
// Output: 60
```

`✅ Passes array elements as individual arguments.`

- `Spreading Objects (Shallow Copy)`

```javascript
const user = { name: "Rishabh", age: 22 };
const updatedUser = { ...user, role: "Developer" };

console.log(updatedUser);
// Output: { name: "Rishabh", age: 22, role: "Developer" }
```

`✅ Copies properties and allows modifications.`

**2. Rest Operator (...) – Collecting Elements**

- `Using Rest in Function Parameters`

```javascript
function add(...numbers) {
  return numbers.reduce((sum, num) => sum + num, 0);
}

console.log(add(10, 20, 30, 40));
// Output: 100
```

`✅ Gathers multiple arguments into an array.`

- ` Rest Operator in Destructuring (Arrays)`

```javascript
const [first, second, ...remaining] = [1, 2, 3, 4, 5];

console.log(first, second); // 1 2
console.log(remaining); // [3, 4, 5]
```

`✅ Extracts first two elements, and the rest goes into an array.`

- ` Rest Operator in Destructuring (Objects)`

```javascript
const user = { name: "Rishabh", age: 22, role: "Developer" };
const { name, ...details } = user;

console.log(name); // "Rishabh"
console.log(details); // { age: 22, role: "Developer" }
```

`✅ Extracts name, and the rest is stored in details.`

## 3. Spread (`...`) vs. Rest (`...`)

| Feature               | Spread (`...`)                  | Rest (`...`)                       |
| --------------------- | ------------------------------- | ---------------------------------- |
| **Purpose**           | Expands elements                | Collects elements                  |
| **Used With**         | Arrays, Objects, Function Calls | Function Parameters, Destructuring |
| **Example (Arrays)**  | `const newArr = [...arr]`       | `[first, ...rest] = arr`           |
| **Example (Objects)** | `{ ...obj }`                    | `{ key, ...rest } = obj`           |

[🔝 Back to Top](#table-of-contents)

## 31. ES6+ Features in JavaScript

ES6 (ECMAScript 2015) and later versions (ES7, ES8, ES9, ES10, etc.) introduced many powerful features that improved JavaScript's readability, maintainability, and performance.

**1. ES6 (ECMAScript 2015) Features**

**`a. let & const (Block-scoped Variables)`**

🔹 let and const provide block-scoped variables, replacing var.

```javascript
let x = 10;
const y = 20;
```

✅ let can be reassigned, but const cannot.

**`b. Template Literals (String Interpolation)`**

🔹 Use backticks `, and embed expressions with ${}.

```javascript
const name = "Rishabh";
console.log(`Hello, ${name}!`);
// Output: Hello, Rishabh!
```

**`c. Arrow Functions (Shorter Function Syntax)`**

🔹 More concise function syntax.

```javascript
const add = (a, b) => a + b;
console.log(add(5, 3)); // Output: 8
```

`✅ Lexical this → Arrow functions do not change the this value.`

**`d. Default Parameters`**

🔹 Provide default values for function parameters.

```javascript
function greet(name = "Guest") {
  console.log(`Hello, ${name}!`);
}
greet(); // Output: Hello, Guest!
```

**`e. Destructuring (Arrays & Objects)`**

🔹 Extract values easily from objects and arrays.

```javascript
const user = { name: "Rishabh", age: 22 };
const { name, age } = user;
console.log(name, age); // Output: Rishabh 22
```

**`f. Spread and Rest Operators (...)`**

🔹 `Spread (...)` → Expands arrays/objects.
🔹 `Rest (...)` → Gathers remaining values into an array.

```javascript
const numbers = [1, 2, 3];
const newNumbers = [...numbers, 4, 5];

function sum(...nums) {
  return nums.reduce((a, b) => a + b);
}
console.log(sum(1, 2, 3)); // Output: 6
```

**`g. Classes (OOP in JavaScript)`**

🔹 class syntax for creating objects.

```javascript
class Person {
  constructor(name) {
    this.name = name;
  }
  greet() {
    console.log(`Hello, ${this.name}`);
  }
}
const person = new Person("Rishabh");
person.greet(); // Output: Hello, Rishabh
```

**`h. Promises (Async Handling)`**

🔹 Handle asynchronous operations without callback hell.

```javascript
const fetchData = () => {
  return new Promise((resolve, reject) => {
    setTimeout(() => resolve("Data received"), 2000);
  });
};
fetchData().then(console.log); // Output (after 2s): Data received
```

## 2. ES7 (ECMAScript 2016) Features

**`a. Exponentiation Operator (**)`\*\*

```javascript
console.log(2 ** 3); // Output: 8
```

**`b. Array.prototype.includes()`**

```javascript
const arr = [10, 20, 30];
console.log(arr.includes(20)); // Output: true
```

## 3. ES8 (ECMAScript 2017) Features

**`a. Async/Await (Simplified Promises)`**

```javascript
async function fetchData() {
  let data = await fetch("https://jsonplaceholder.typicode.com/todos/1");
  let json = await data.json();
  console.log(json);
}
fetchData();
```

**`b.  Object.entries() & Object.values()`**

```javascript
const user = { name: "Rishabh", age: 22 };
console.log(Object.entries(user)); // Output: [["name", "Rishabh"], ["age", 22]]
console.log(Object.values(user)); // Output: ["Rishabh", 22]
```

## 4. ES9 (ECMAScript 2018) Features

**`a. Rest/Spread for Objects`**

```javascript
const user = { name: "Rishabh", age: 22, city: "Delhi" };
const { city, ...details } = user;
console.log(details); // Output: { name: "Rishabh", age: 22 }
```

## 5. ES10 (ECMAScript 2019) Features

**`Optional Catch Binding`**

```javascript
try {
  throw "Error!";
} catch {
  console.log("Caught an error!");
}
```

## 6. ES11 (ECMAScript 2020) Features

**`a. Optional Chaining (?.)`**

```javascript
const user = { profile: { name: "Rishabh" } };
console.log(user.profile?.name); // Output: Rishabh
console.log(user.address?.city); // Output: undefined
```

**`b. Nullish Coalescing (??)`**

```javascript
const user = null;
console.log(user ?? "Guest"); // Output: Guest
```

## ES12 (ECMAScript 2021) Features

**`a. Replace All (.replaceAll())`**

```javascript
const str = "Hello World, Hello JavaScript!";
console.log(str.replaceAll("Hello", "Hi"));
// Output: Hi World, Hi JavaScript!
```

[🔝 Back to Top](#table-of-contents)

## 32. Error Handling in JavaScript

JavaScript provides a mechanism for handling errors using the try-catch-finally block. This ensures that code execution doesn't stop unexpectedly when an error occurs.

**1. Understanding try-catch-finally**

| Block     | Purpose                                         |
| --------- | ----------------------------------------------- |
| `try`     | Code that might throw an error.                 |
| `catch`   | Handles errors from the `try` block.            |
| `finally` | Executes code **always**, regardless of errors. |

- `Basic Example`

```javascript
try {
  console.log(x); // Error: x is not defined
} catch (error) {
  console.log("An error occurred:", error.message);
} finally {
  console.log("This will always execute.");
}
```

- ✅ If an error occurs in try, catch handles it.
- ✅ finally runs whether an error occurs or not.

- `Output:`

```javascript
An error occurred: x is not defined
This will always execute.
```

**2. Handling Specific Errors**

- JavaScript provides different error types, such as `ReferenceError`, `TypeError`, and `SyntaxError`.

- `Handling Specific Errors`

```javascript
try {
  let num = 5;
  num.toUpperCase(); // TypeError
} catch (error) {
  if (error instanceof TypeError) {
    console.log("Type Error:", error.message);
  } else {
    console.log("Some other error occurred.");
  }
}
```

- ✅ instanceof checks for specific error types.

**3. Throwing Custom Errors**

You can manually throw errors using throw.

- `Throw Custom Errors`

```javascript
function divide(a, b) {
  if (b === 0) {
    throw new Error("Division by zero is not allowed.");
  }
  return a / b;
}

try {
  console.log(divide(10, 0));
} catch (error) {
  console.log("Error:", error.message);
}
```

- ✅ throw creates custom errors, which can be handled in catch.

**4. Nested try-catch**

- You can use nested try-catch for handling multiple levels of errors.

```javascript
try {
  try {
    JSON.parse("{invalidJson}");
  } catch (error) {
    console.log("Inner catch:", error.message);
    throw new Error("Re-throwing error"); // Throwing it again
  }
} catch (error) {
  console.log("Outer catch:", error.message);
}
```

- ✅ Inner catch handles the first error, then re-throws it to the outer catch.

**5. Using finally for Cleanup**

- The finally block is useful for closing connections, releasing resources, etc.

```javascript
function fetchData() {
  try {
    console.log("Fetching data...");
    throw new Error("Network Error");
  } catch (error) {
    console.log("Caught an error:", error.message);
  } finally {
    console.log("Cleaning up resources...");
  }
}

fetchData();
```

- ✅ Even if an error occurs, finally always runs.

**6. try-catch with Asynchronous Code**

- When handling async operations, you must use try-catch inside async/await functions.

- `Handling Errors in Async Code`

```javascript
async function fetchData() {
  try {
    let response = await fetch("invalid-url");
    let data = await response.json();
    console.log(data);
  } catch (error) {
    console.log("Async Error:", error.message);
  }
}

fetchData();
```

- ✅ catch handles async errors inside an async function.

[🔝 Back to Top](#table-of-contents)

## 33. Promises in JavaScript

A Promise in JavaScript is an object that represents the eventual completion (or failure) of an asynchronous operation. It helps in handling asynchronous operations in a cleaner way compared to callback functions.

**1. Understanding Promises**

`Promise States in JavaScript`

| State         | Description                                    |
| ------------- | ---------------------------------------------- |
| **Pending**   | Initial state, neither fulfilled nor rejected. |
| **Fulfilled** | The operation completed successfully.          |
| **Rejected**  | The operation failed.                          |

` Basic Syntax of a Promise`

```javascript
const myPromise = new Promise((resolve, reject) => {
  let success = true; // Change this to false to test rejection
  if (success) {
    resolve("Operation Successful!");
  } else {
    reject("Operation Failed!");
  }
});
```

**2. Handling Promises with `.then()` and `.catch()`**

`Using .then() for Success and .catch() for Errors`

```javascript
const myPromise = new Promise((resolve, reject) => {
  let success = true; // Change this to false to test rejection
  if (success) {
    resolve("Operation Successful!");
  } else {
    reject("Operation Failed!");
  }
});

myPromise
  .then((message) => {
    console.log("Success:", message);
  })
  .catch((error) => {
    console.log("Error:", error);
  });
```

- ✅ .then() executes if the promise is resolved.
- ✅ .catch() executes if the promise is rejected.

**3. Chaining Promises**

Multiple .then() can be chained to handle sequential asynchronous tasks.

```javascript
new Promise((resolve) => {
  setTimeout(() => resolve(10), 1000);
})
  .then((num) => {
    console.log("First:", num);
    return num * 2;
  })
  .then((num) => {
    console.log("Second:", num);
    return num * 3;
  })
  .then((num) => {
    console.log("Third:", num);
  })
  .catch((error) => console.log("Error:", error));
```

- ✅ This ensures operations execute one after another.

`Output:`

```javascript
First: 10;
Second: 20;
Third: 60;
```

**4. Promise.all() – Execute Multiple Promises in Parallel**

Used when multiple promises need to be resolved before proceeding.

```javascript
const promise1 = new Promise((resolve) =>
  setTimeout(() => resolve("Task 1"), 2000)
);
const promise2 = new Promise((resolve) =>
  setTimeout(() => resolve("Task 2"), 1000)
);

Promise.all([promise1, promise2]).then((values) => {
  console.log("All Promises Resolved:", values);
});
```

- ✅ If all promises resolve, it returns an array of results.
- ❌ If any promise fails, Promise.all() rejects immediately.

**5. Promise.race() – First Resolved Promise Wins**

Returns the first settled (resolved/rejected) promise.

```javascript
Promise.race([
  new Promise((resolve) => setTimeout(() => resolve("Fastest"), 1000)),
  new Promise((resolve) => setTimeout(() => resolve("Slow"), 2000)),
]).then((value) => {
  console.log("First Resolved:", value);
});
```

- ✅ The fastest promise resolves first.

**6. Converting Callbacks to Promises**

A common use case of promises is converting callback-based code into promise-based.

`Example: setTimeout with Promise`

```javascript
function delay(ms) {
  return new Promise((resolve) => setTimeout(resolve, ms));
}

delay(2000).then(() => console.log("Executed after 2 seconds"));
```

- ✅ This helps avoid callback hell.

**7. Async/Await with Promises**

Promises work well with async/await, making async code look synchronous.

```javascript
async function fetchData() {
  try {
    let response = await new Promise((resolve) =>
      setTimeout(() => resolve("Data received"), 2000)
    );
    console.log(response);
  } catch (error) {
    console.log("Error:", error);
  }
}

fetchData();
```

- ✅ await waits for the promise to resolve.
- ✅ try-catch handles errors gracefully.

[🔝 Back to Top](#table-of-contents)

## 34. Async/Await in JavaScript

async/await is a modern way to handle asynchronous code in JavaScript. It simplifies working with Promises and makes asynchronous code look more like synchronous code.

**1. Understanding async and await**

| Keyword | Purpose                                                    |
| ------- | ---------------------------------------------------------- |
| `async` | Defines a function that always returns a promise.          |
| `await` | Waits for a promise to resolve inside an `async` function. |

**2. Example of async/await**

```javascript
async function fetchData() {
  return "Hello, World!";
}

fetchData().then(console.log); // Output: Hello, World!
```

- ✅ The function fetchData automatically returns a Promise because it is marked async.

**3. Using await to Handle Promises**

await is used to pause execution until a promise resolves.

```javascript
function fetchData() {
  return new Promise((resolve) => {
    setTimeout(() => resolve("Data received!"), 2000);
  });
}

async function getData() {
  console.log("Fetching data...");
  let result = await fetchData();
  console.log(result);
}

getData();
```

`Output:`

```javascript
Fetching data...
(Data appears after 2 seconds)
Data received!
```

- ✅ await waits for the promise to resolve before moving to the next line.

**4. Handling Errors in async/await with try-catch**

```javascript
async function fetchData() {
  try {
    let response = await fetch("invalid-url"); // This will fail
    let data = await response.json();
    console.log(data);
  } catch (error) {
    console.log("Error:", error.message);
  }
}

fetchData();
```

- ✅ try-catch handles errors gracefully in async functions.

**5. Parallel Execution using Promise.all() in async/await**

To improve performance, we can execute multiple promises simultaneously.

```javascript
async function fetchAllData() {
  let [data1, data2] = await Promise.all([
    fetch("https://jsonplaceholder.typicode.com/todos/1").then((res) =>
      res.json()
    ),
    fetch("https://jsonplaceholder.typicode.com/todos/2").then((res) =>
      res.json()
    ),
  ]);

  console.log(data1, data2);
}

fetchAllData();
```

- ✅ Promise.all() executes requests in parallel instead of sequentially.

**6. await Inside Loops**

Using await inside loops must be done carefully to avoid unnecessary delays.

❌ Bad Approach (Executes One by One)

```javascript
async function processItems(items) {
  for (let item of items) {
    await fetchData(item); // Each request waits for the previous one to complete
  }
}
```

✅ Optimized Approach (Executes in Parallel)

```javascript
async function processItems(items) {
  let promises = items.map(fetchData);
  await Promise.all(promises);
}
```

- ✅ This ensures all fetch operations run simultaneously.

[🔝 Back to Top](#table-of-contents)

## 35. Difference between async/await and .then() in promises

**1. Syntax & Readability**

- `.then() (Promise Chaining)`

  - Uses method chaining.

  - Can lead to nested code when handling multiple promises.

  ```javascript
  fetch("https://jsonplaceholder.typicode.com/todos/1")
    .then((response) => response.json())
    .then((data) => console.log(data))
    .catch((error) => console.log("Error:", error));
  ```

- `async/await (Synchronous-like Flow)`

  - Looks more like synchronous code.

  - Easier to read and maintain.

  ```javascript
  async function fetchData() {
    try {
      let response = await fetch(
        "https://jsonplaceholder.typicode.com/todos/1"
      );
      let data = await response.json();
      console.log(data);
    } catch (error) {
      console.log("Error:", error);
    }
  }

  fetchData();
  ```

  - ✅ async/await improves readability and avoids callback nesting.

**2. Error Handling**

- `.then().catch()`

  - Uses .catch() at the end to handle errors.

  - If there's an error anywhere in the chain, it goes directly to .catch().

  ```javascript
  fetch("invalid-url")
    .then((response) => response.json())
    .then((data) => console.log(data))
    .catch((error) => console.log("Error:", error.message));
  ```

- `async/await with try-catch`

  - Requires try-catch inside async functions.

  - Can handle errors locally at each step.

  ```javascript
  async function fetchData() {
    try {
      let response = await fetch("invalid-url");
      let data = await response.json();
      console.log(data);
    } catch (error) {
      console.log("Error:", error.message);
    }
  }

  fetchData();
  ```
  - ✅ async/await provides better error handling since errors can be caught at multiple points.

**3. Handling Multiple Promises**

- `.then() (Promise.all)`

```javascript
Promise.all([
  fetch("https://jsonplaceholder.typicode.com/todos/1").then((res) =>
    res.json()
  ),
  fetch("https://jsonplaceholder.typicode.com/todos/2").then((res) =>
    res.json()
  ),
]).then(([data1, data2]) => {
  console.log(data1, data2);
});
```

- `async/await (Promise.all with await)`

```javascript
async function fetchAllData() {
  let [data1, data2] = await Promise.all([
    fetch("https://jsonplaceholder.typicode.com/todos/1").then((res) =>
      res.json()
    ),
    fetch("https://jsonplaceholder.typicode.com/todos/2").then((res) =>
      res.json()
    ),
  ]);

  console.log(data1, data2);
}

fetchAllData();
```

- ✅ Both approaches can handle multiple promises, but async/await is cleaner.

**4. Execution & Performance**

- `.then()` executes asynchronously but continues execution without waiting for the promise to resolve.

- `async/await` pauses execution at each await until the promise resolves.

- ✅ `Promise.all()` should be used in both cases when executing multiple independent promises to avoid blocking.

[🔝 Back to Top](#table-of-contents)
