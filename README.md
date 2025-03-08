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

## 8. What is Template Literal

Template literals are string literals that allow embedded expressions (variables) into your code. They are enclosed by backticks (`) instead of single (‘) or double (“) quotes.

- It was introduced in ES6, which provides a more flexible and readable way to work with strings.

```
let a='GFG'
console.log(`hello ${a}`)

```

## 7. What is String

- A string (or a text string) is a series of characters like "Rishabh Kashyap".

Strings are written with quotes. You can use single or double quotes.

```
const string1 = "A string primitive";
const string2 = 'Also a string primitive';

```

**Character access**

```
"cat".charAt(1); // gives value "a"
"cat"[1]; // gives value "a"
```

**String objects**

```
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

```
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

```
const sentence = "The quick brown fox jumps over the lazy dog.";

const index = 4;

console.log(`The character at index ${index} is ${sentence.charAt(index)}`);
// Expected output: "The character at index 4 is q"

```

- **String.prototype.charCodeAt()**

The charCodeAt() method of String values returns an integer between 0 and 65535

```
const index = 4;

console.log(
 `Character code ${sentence.charCodeAt(index)} is equal to ${sentence.charAt(
   index,
 )}`,
);
// Expected output: "Character code 113 is equal to q"
```

- **String.concat()**

The concat() method of String values concatenates the string arguments to this string and returns a new string.

```
const str1 = "Hello";
const str2 = "World";

console.log(str1.concat(" ", str2));
// Expected output: "Hello World"

console.log(str2.concat(", ", str1));
// Expected output: "World, Hello"
```

- **String.endsWith()**

The endsWith() method of String values determines whether a string ends with the characters of this string, returning true or false as appropriate.

```
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

```
const sentence = "The quick brown fox jumps over the lazy dog.";

const word = "fox";

console.log(
 `The word "${word}" ${
   sentence.includes(word) ? "is" : "is not"
 } in the sentence`,
)
```

- **String.indexOf()**

```const paragraph = "I think Ruth's dog is cuter than your dog!";

const searchTerm = "dog";
const indexOfFirst = paragraph.indexOf(searchTerm);

console.log(`The index of the first "${searchTerm}" is ${indexOfFirst}`);
// Expected output: "The index of the first "dog" is 15"

console.log(
  `The index of the second "${searchTerm}" is ${paragraph.indexOf(
    searchTerm,
    indexOfFirst + 1,
  )}`,
);
// Expected output: "The index of the second "dog" is 38"
```

- **String.lastIndexOf()**

```
const paragraph = "I think Ruth's dog is cuter than your dog!";

const searchTerm = "dog";

console.log(
  `Index of the last ${searchTerm} is ${paragraph.lastIndexOf(searchTerm)}`,
);
// Expected output: "Index of the last "dog" is 38"
```

- **String.localeCompare()**

```
const a = "réservé"; // With accents, lowercase
const b = "RESERVE"; // No accents, uppercase

console.log(a.localeCompare(b));
// Expected output: 1
```

- **String.repeat()**

```
const mood = "Happy! ";

console.log(`I feel ${mood.repeat(3)}`);
// Expected output: "I feel Happy! Happy! Happy! "
```

- **String.replace()**

The original string is left unchanged.

```
const paragraph = "I think Ruth's dog is cuter than your dog!";

console.log(paragraph.replace("Ruth's", "my"));
// Expected output: "I think my dog is cuter than your dog!"
```

- **String.replaceAll()**

The replaceAll() method of String values returns a new string with all matches of a pattern replaced by a replacement.

```
const paragraph = "I think Ruth's dog is cuter than your dog!";

console.log(paragraph.replaceAll("dog", "monkey"));
// Expected output: "I think Ruth's monkey is cuter than your monkey!"
```

- **String.slice()**

The slice() method of String values extracts a section of this string and returns it as a new string, without modifying the original string.

```
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

```
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

```
const str = "The morning is upon us.";
str.slice(-3); // 'us.'
str.slice(-3, -1); // 'us'
str.slice(0, -1); // 'The morning is upon us'
str.slice(4, -1); // 'morning is upon us'
```

- **String.split()**

```
const str = "The quick brown fox jumps over the lazy dog.";

const words = str.split(" ");
console.log(words[3]);
// Expected output: "fox"

const chars = str.split("");
console.log(chars[8]);
// Expected output: "k"
```

```
const emptyString = "";

// string is empty and separator is non-empty
console.log(emptyString.split("a"));
// [""]

// string and separator are both empty strings
console.log(emptyString.split(emptyString));
// []
```

```
const myString = "Hello World. How are you doing?";
const splits = myString.split(" ", 3);

console.log(splits); // [ "Hello", "World.", "How" ]
```

- **String.startsWith()**

```
const str1 = "Saturday night plans";

console.log(str1.startsWith("Sat"));
// Expected output: true

console.log(str1.startsWith("Sat", 3));
// Expected output: false
```

- **String.substring()**

```
const str = "Mozilla";

console.log(str.substring(1, 3));
// Expected output: "oz"

console.log(str.substring(2));
// Expected output: "zilla"
```

- **String.toLowerCase()**

The toLowerCase() method of String values returns this string converted to lower case.

```
const sentence = "The quick brown fox jumps over the lazy dog.";

console.log(sentence.toLowerCase());
// Expected output: "the quick brown fox jumps over the lazy dog."
```

- **String.toUpperCase()**

The toUpperCase() method of String values returns this string converted to uppercase.

```
const sentence = "The quick brown fox jumps over the lazy dog.";

console.log(sentence.toUpperCase());
// Expected output: "THE QUICK BROWN FOX JUMPS OVER THE LAZY DOG."
```

- **String.trim()**

The trim() method of String values removes whitespace from both ends of this string and returns a new string, without modifying the original string.

```
const greeting = "   Hello world!   ";

console.log(greeting);
// Expected output: "   Hello world!   ";

console.log(greeting.trim());
// Expected output: "Hello world!";

```

- **String.trimEnd()**

```
const greeting = "   Hello world!   ";

console.log(greeting);
// Expected output: "   Hello world!   ";

console.log(greeting.trimEnd());
// Expected output: "   Hello world!";
```

- **String.trimStart()**

```
const greeting = "   Hello world!   ";

console.log(greeting);
// Expected output: "   Hello world!   ";

console.log(greeting.trimStart());
// Expected output: "Hello world!   ";
```

- **String.valueOf()**

```

const stringObj = new String("foo");
console.log(stringObj.valueOf());
// Expected output: "foo"
```

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
