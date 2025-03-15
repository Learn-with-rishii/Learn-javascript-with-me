# Learn-javascript-with-me

### Table of Contents

<!-- TOC_START -->

| No. | Questions                                                                                                |
| --- | -------------------------------------------------------------------------------------------------------- |
| 1   | [What is JavaScript?](#1-what-is-javascript)                                                             |
| 2   | [Why Study JavaScript?](#2-why-study-javascript)                                                         |
| 3   | [JavaScript Variables](#3-javascript-variables)                                                          |
| 4   | [var/let/const](#4-varletconst)                                                                          |
| 5   | [Difference Between var, let and const](#5-difference-between-var-let-and-const)                         |
| 6   | [JavaScript Data Types](#6-javascript-data-types)                                                        |
| 7   | [What is String](#7-what-is-string)                                                                      |
| 8   | [What is Array](#8-what-is-array)                                                                        |
| 9   | [What is forEach](#9-what-is-foreach)                                                                    |
| 10  | [ Differences Between `forEach()` and Other Loops](#10-differences-between-foreach-and-other-loops)      |
| 11  | [ What is Map in JavaScript](#11-what-is-map-in-javascript)                                              |
| 12  | [What is the filter Function](#12-what-is-the-filter-function)                                           |
| 13  | [ Difference between filter , map , foreach](#13-difference-between-filter--map--foreach)                |
| 14  | [ What is the reduce Function](#14-what-is-the-reduce-function)                                          |
| 15  | [Difference Between `reduce()` vs `map()` vs `filter()`](#15-difference-between-reduce-vs-map-vs-filter) |
| 16  | [What is an Object in JavaScript](#16-what-is-an-object-in-javascript)                                   |

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

```

```

```

```
