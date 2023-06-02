# Java scrip

# Java Script(JS)

Java Script is a high-level, dynamic, interpreted programming language that is used to make web pages interactive and dynamic. 

It is often abbreviated as **JS**.

 It is a client-side scripting language that is mainly used for creating web pages and applications. Java Script is used in conjunction with **HTML** and **CSS** to create interactive and dynamic web pages. It is supported by all popular web browsers and can also be used on the server side through platforms such as Node.js.

Java Script is a versatile language that can be used for a range of applications such as creating web and mobile applications, games, and server-side applications. 

It is an object-oriented language that uses objects to represent and manipulate data.

 Java Script is also known for its ability to manipulate the **Document Object Model (DOM)** which allows developers to change the structure, content, and style of web pages dynamically.

Overall, Java Script is a popular programming language that is widely used in the development of web applications. Its versatility, ease of use, and wide range of applications make it an essential tool for web developers.

# Variable in JS

Variables are Containers for Storing Data, Variables are containers for storing values.

JavaScript Variables can be declared in 4 ways:

- Automatically
- Using `var`
- Using `let`
- Using `const`

**NOTE:** The `var` keyword was used in all JavaScript code from 1995 to 2015, and should only be    used in code written for older browsers.

           The `let` and `const` keywords were added to JavaScript in 2015.

# When to Use var, let, or const?

1. Always declare variables

2. Always use `const` if the value should not be changed

3. Always use `const` if the type should not be changed (Arrays and Objects)

4. Only use `let` if you can't use `const`

5. Only use `var` if you MUST support old browsers.

# Data type in JS

A JavaScript variable can hold any type of data.                                 

| JavaScript has 8 Datatypes   | The Object Datatype:  |
| --- | --- |
| 1. String | 1. An object |
| 2. Number | 2. An array |
| 3. Bigint | 3. A date |
| 4. Boolean |  |
| 5. Undefined |  |
| 6. Null |  |
| 7. Symbol |  |
| 8. Object |  |

The data type can be classified into two ways:

- Primitive
- Regular(non-primitive)

### Primitive data type

In JavaScript, primitive data types are the basic data types that are not objects and do not have any properties. 

*Primitive* data types are immutable(non-modifiable) data types. Once a primitive data type is created we cannot modify it.

The six primitive data types in JavaScript are: 

1. String
2. Number
3. Boolean
4. Null
5. Undefined
6. Symbol

### Regular(non-primitive) data type

Non-primitive data types, also called reference data types, are more complex than primitive data types and are objects. They are called reference types because they refer to memory locations and therefore can be quite large.

*Non-primitive* data types are modifiable or mutable. We can modify the value of non-primitive data types after it gets created.

When we say Non-primitive data type is regular because they are being compared by reference instead of value.

The non-primitive data types include:
1. Objects (including arrays and functions)
2. Dates
3. Regular expressions

# Data string in JS

In JavaScript, a string is a sequence of characters enclosed in single or double quotation marks. It is a primitive data type that represents textual data. 

**Strings** are commonly used to store and manipulate text in JavaScript. 
For example, you can assign a string to a variable like this:

```jsx
let greeting = "Hello, World!";
```

In this example, the string "Hello, World!" is assigned to the variable `greeting`. You can access individual characters in a string using indexing, just like you would with an array.

For example, to access the first letter of the `greeting` variable above, you could use:

```jsx
let firstLetter = greeting[0]; // firstLetter will be "H"
```

You can also concatenate strings using the plus (`+`) operator:

```jsx
let name = "smith";
let greeting = "Hello, " + name + "!";
console.log(greeting); // logs "Hello, smith!"
```

# Data Structure in JS

JavaScript data structures are containers used to organize and store data. They can be classified into two categories: built-in data structures and user-defined data structures.

1. Built-In Data Structures: JavaScript provides a few built-in data structures, which include:
- Array: An array is a collection of elements that are ordered, and can be accessed using indices.
- Object: An object is a collection of properties that have key-value pairs.
- Map: A map is a collection of key-value pairs that can use any type of value as a key or value.
- Set: A set is a collection of unique values.
1. User-Defined Data Structures: In addition to built-in data structures, JavaScript allows developers to create their custom data structures using classes or constructor functions. For example, you could create a linked list or binary search tree data structure in JavaScript.

These data structures can help you efficiently manage and manipulate large amounts of data in your programs. Depending on the problem you want to solve, different data structures may be more appropriate to use than others.

# Control Loop in JS

In Javascript, a control loop is a set of statements that are executed repeatedly until a condition is met. 

There are three types of control structures in JavaScript: 

For loop: is typically used when you know how many times the loop should be executed.

While loop: while loop is used when you want to continue looping until a certain condition is met.

Do-while loop: is similar to the while loop, but it always executes at least once before checking the condition. 

# Function in JS

A function is a reusable block of code or programming statements designed to perform a certain task. A function is declared by a function keyword followed by a name, followed by parentheses (). AParenthesescan take a parameter. If a function take a parameter it will be called with argument. A function can also take a default parameter. To store data to a function, a function has to return certain data types. To get the value we call or invoke a function. 

FuThe functionakes code:

- clean and easy to read
- reusable
- easy to test

A function can be declared or created in couple of ways:

- *Declaration function*
- *Expression function*
- *Anonymous function*
- *Arrow function*

### Function Declaration

Let us see how to declare a function and how to call a function.

```flow
//declaring a function without a parameter
function functionName() {
  // code goes here
}
functionName() // calling function by its name and with parentheses
```

**Function without a parameter and returThe function**

Function can be declared without a parameter.

```flow
// function without parameter,  a fumakeson which makes a number square
function square() {
  let num = 2
  let sq = num * num
  console.log(sq)
}

square() // 4

// function without parameter
function addTwoNumbers() {
  let numen = 10
  let numTwo = 20
  let sum = numOne + numTwo

  console.log(sum)
}

addTwoNumbers() // a function has to be called by its name to be executed
```

**Function with a parameter**

In a function we can pass different data types(number, string, boolean, object, function) as a parameter.

```flow
// function with one parameter
function functionName(parm1) {
  //code goes her
}
functionName(parm1) // during calling or invoking one argument needed

function areaOfCircle(r) {
  let area = Math.PI * r * r
  return area
}

console.log(areaOfCircle(10)) // should be called with one argument

function square(number) {
  return number * number
}

console.log(square(10))
```

### Expression Function

Expression functions are **anonymous functions.** After we create a function without a name and we assign it to a variable. To return a value from the function we should call the variable. Look at the example below.

```flow
// Function expression
const square = function(n) {
  return n * n
}

console.log(square(2)) // -> 4
```

### Anonymous Function

Anonymous function or without name

```flow
const anonymousFun = function() {
  console.log(
    'I am an anonymous function and my value is stored in anonymousFun'
  )
}
```

### Arrow Function

The arrow function is an alternative to writing a function, however, function declaration and arrow function have some minor differences.

The arrow function uses the arrow instead of the keyword *function* to declare a function. Let us see both function declaration and arrow function.

# Boolean in JS

A boolean data type represents one of the two values: *true* or *false*. 

The default value of the boolean is false.

| Truthy values | False values |
| --- | --- |
| All numbers(positive and negative) are truthy except zero | 0 |
|  All strings are truthy except an empty string ('') | 0n |
| The boolean true | null |
|  | undefined |
|  | NaN |
|  | the boolean false |
|  | '', "", ``, empty string |

# **Conditionals in JS**

Conditional statements are used to make decisions based on different conditions. By default, statements in JavaScript script are executed sequentially from top to bottom. If the processing logic requires so, the sequential flow of execution can be altered in two ways:

- **Conditional execution:** a block of one or more statements will be executed if a certain expression is true
- **Repetitive execution:** a block of one or more statements will be repetitively executed as long as a certain expression is true. In this section, we will cover *if*, *else*, and *else if* statements. The comparison and logical operators we learned in the previous sections will be useful in here.

Conditions can be implemented using the following ways:

- if
- if else
- if else if else
- switch

**if**

In JavaScript and other programming languages the keyword *if* is to used check if a condition is true and to execute the block code. To create an if condition, we need an *if* keyword, a condition inside a parent, a thesis, and a block of code inside a curly bracket({}).

```flow
// syntax
if (condition) {
  //this part of the code runs for truthy condition
}
```

### If Else

If the condition is true the first block will be executed, if not the else condition will be executed.

```flow
// syntax
if (condition) {
  // This part of the code runs for truthy condition
} else {
  //This part of the code runs for false condition
}
```

### If Else if Else

On our daily life, we make decisions on daily basis. We make decisions not by checking one or two conditions instead we make decisions based on multiple conditions. Similar to our daily life, programming is also full of conditions. We use *else* when we have multiple conditions.

```flow
// syntax
if (condition) {
     // code
} else if (condition) {
   // code
} else {
    //  code

}
```

### Switch

Switch is an alternative for **if else if else else**. The switch statement starts with a *switch* keyword followed by a parenthesis and code block. Inside the code block, we will have different cases. Case block runs if the value in the switch statement parenthesis matches with the case value. The break statement is to terminate execution so the code execution does not go down after the condition is satisfied. The default block runs if all the cases don't satisfy the condition.

```flow
switch(caseValue){
  case 1:
    // code
    break
  case 2:
   // code
   break
  case 3:
   // code
   break
  default:
   // code
}
```

# Array in JS

An array is a collection of different data types which are ordered and changeable(modifiable). An array allows for storing duplicate elements and different data types. An array can be empty, or it may have different data type values.

### How to create an empty array

In JavaScript, we can create an array in different ways. Let us see different ways to create an array. It is very common to use *const* instead of *let* to declare an array variable. If you are using const it means you do not use that variable name again.

• Using Array constructor

```flow
// syntax
const arr = Array()
// or
// let arr = new Array()
console.log(arr) // []
```

• Using square brackets([])

```flow
// syntax
// This the most recommended way to create an empty list
const arr = []
console.log(arr)
```

### How to create an array with values

Array with initial values. We use *length* property to find the length of an array.

• Array can have items of different data types

```flow
const arr = [
    'Asabeneh',
    250,
    true,
    { country: 'Finland', city: 'Helsinki' },
    { skills: ['HTML', 'CSS', 'JS', 'React', 'Python'] }
] // arr containing different data types
console.log(arr)
```

# Scope in JS

Variable is the fundamental part in programming. We declare variable to store different data types. To declare a variable we use the key word *var*, *let* and *const*. A variable can be declared at different scope. In this section, we will see the scope variables, scope of variables when we use var or let. Variables scopes can be:

- Global
- Local

### Global scope

A globally declared variable can be accessed every where in the same file. But the term global is relative. It can be global to the file or it can be global relative to some block of codes.

```flow
//scope.js
let a = 'JavaScript' // is a global scope it will be found anywhere in this file
let b = 10 // is a global scope it will be found anywhere in this file
function letsLearnScope() {
  console.log(a, b) // JavaScript 10, accessible
  if (true) {
    let a = 'Python'
    let b = 100
    console.log(a, b) // Python 100
  }
  console.log(a, b)
}
letsLearnScope()
console.log(a, b) // JavaScript 10, accessible
```

### Local scope

A variable declared as local can be accessed only in certain block code.

- Block Scope
- Function Scope

```flow
//scope.js
let a = 'JavaScript' // is a global scope it will be found anywhere in this file
let b = 10 // is a global scope it will be found anywhere in this file
// Function scope
function letsLearnScope() {
  console.log(a, b) // JavaScript 10, accessible
  let value = false
// block scope
  if (true) {
    // we can access from the function and outside the function but 
    // variables declared inside the if will not be accessed outside the if block
    let a = 'Python'
    let b = 20
    let c = 30
    let d = 40
    value = !value
    console.log(a, b, c, value) // Python 20 30 true
  }
  // we can not access c because c's scope is only the if block
  console.log(a, b, value) // JavaScript 10 true
}
letsLearnScope()
console.log(a, b) // JavaScript 10, accessible
```

## Object

Everything can be an object and objects do have properties and properties have values, so an object is a key value pair. The order of the key is not reserved, or there is no order. To create an object literal, we use two curly brackets.

```flow
const person = {}
```

## **Classes**

To define a class in JavaScript we need the keyword *class* , the name of a class in **CamelCase** and block code(two curly brackets).

```flow
// syntax
class ClassName {
    //  code goes here
}
```

### Class Instantiation

Instantiation class means creating an object from a class. We need the keyword *new* and we call the name of the class after the word new.

```flow
class Person {
  // code goes here
}
const person = new Person()
console.log(person)
```

### Class Constructor

The constructor is a builtin function which allows as to create a blueprint for our object. The constructor function starts with a keyword constructor followed by a parenthesis. Inside the parenthesis we pass the properties of the object as parameter. We use the ***this*** keyword to attach the constructor parameters with the class.

```flow
class Person {
  constructor(firstName, lastName) {
    console.log(this) // Check the output from here
    this.firstName = firstName
    this.lastName = lastName
  }
}

const person = new Person()

console.log(person)

//output

Person {firstName: undefined, lastName:undefined}
```

# **Higher Order Function**

Higher order functions are functions which take other function as a parameter or return a function as a value. The function passed as a parameter is called callback.

### Callback

A callback is a function which can be passed as parameter to other function.

```flow
// a callback function, the name of the function could be any name
const callback = (n) => {
  return n ** 2
}

// function that takes other function as a callback
function cube(callback, n) {
  return callback(n) * n
}

console.log(cube(callback, 3))
```

### Returning function

Higher order functions return function as a value

```flow
// Higher order function returning an other function
const higherOrder = n => {
  const doSomething = m => {
    const doWhatEver = t => {
      return 2 * n + 3 * m + t
    }
    return doWhatEver
  }
  return doSomething
}
console.log(higherOrder(2)(3)(10))
```

### Setting time

In JavaScript, we can execute some activities in a certain interval of time or we can schedule(wait) for some time to execute some activities.

- setInterval
- setTimeout

### Setting Interval using a setInterval function

In JavaScript, we use the setInterval higher-order function to do some activity continuously within some interval of time. The setInterval global method takes a callback function and a duration as a parameter. The duration is in milliseconds and the callback will be always called in that interval of time.

```flow
// syntax
function callback() {
  // code goes here
}
setInterval(callback, duration)
```

### Setting a time using a setTimeout

In JavaScript, we use the setTimeout higher-order function to execute some action at some time in the future. The setTimeout global method takes a callback function and a duration as a parameter. The duration is in milliseconds and the callback waits for that amount of time.

```flow
// syntax
function callback() {
  // code goes here
}
setTimeout(callback, duration) // duration in milliseconds
```