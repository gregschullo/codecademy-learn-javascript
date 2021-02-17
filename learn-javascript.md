---
id: learn-javascript
title: Learn Javascript
---

These notes are derived from [Codecademy Course - Learn JavaScript](https://www.codecademy.com/learn/introduction-to-javascript) course and example exercises.  

## JavaScript Basics

### What is JavaScript?

JavaScript is primarily known as the language of most modern web browsers.  
JavaScript is a powerful, flexible, and fast programming language used for complex web development and more.  
JavaScript powers the dynamic behaviors of most websites.  

### Console

The console is a panel that displays important messages, like errors, for developers. Much of the work the computer does with the code we write us invisible to us by default. We can make things appear on our screen by printing, or logging, to the console directly.  

**keyword** - words that are built into the JavaScript language, so the computer will recognize them and treat them specially.  

**console** - a JavaScript keyword that refers to an object (a collection of data and actions), we can use in our code.  

The `log()` method is built in to the console object. When you write `console.log(value)` value will get printed, or logged, to the console.  

In JavaScript, it is recommended to end each statement with a semicolon (;).  

### Comments

In JavaScript, we can write comments in our code that the computer will ignore as our program runs. These comments exist just for human readers.  
Comments can explain what the code is doing, leave instructions for developers using the code, or add any other useful annotations.  

There are two types of code comments in JavaScript:

A single line comment will comment out a single line and is denoted with two forward slashes `//` preceding it.  
You can also use a single line comment to comment after a line of code.  

A multi-line comment will comment out multiple lines and is denoted with `/*` to begin the comment, and `*/` to end the comment.  

### Data Types

Data types are the classifications for the different kinds of data that we use in programming. In JavaScript, there are seven fundamental data types:

- Number
    Any number, including numbers with decimals: 4, 8, 1516, 23.42.
- String
    Any grouping of characters on your keyboard (letters, numbers, spaces, symbols, etc.) surrounded by single quotes: ' ... ' or double quotes " ... ". Though we prefer single quotes. Some people like to think of string as a fancy word for text.
- Boolean
    This data type only has two possible values— either true or false (without quotes). It’s helpful to think of booleans as on and off switches or as the answers to a “yes” or “no” question.
- Null
    This data type represents the intentional absence of a value, and is represented by the keyword null (without quotes).
- Undefined
    This data type is denoted by the keyword undefined (without quotes). It also represents the absence of a value though it has a different use than null.
- Symbol
    A newer feature to the language, symbols are unique identifiers, useful in more complex coding. No need to worry about these for now.
- Object
    Collections of related data.

The first 6 of those types are considered *primitive data types*. They are the most basic data types in the language. Objects are more complex.  

### Arithmetic Operators

An operator is a character that performs a task in our code. JavaScript has several built-in in arithmetic operators, that allow us to perform mathematical calculations on numbers. These include the following operators and their corresponding symbols:

Add: +  
Subtract: -  
Multiply: *  
Divide: /  
Remainder: %  

### String Concatenation

When a `+` operator is used between two strings, it appends the right string to the left string.  
**concatenation** - the process of appending one string to another.  

### Properties

Every string instance has a property called length that stores the number of characters in that string. You can retrieve property information by appending the string with a period and the property name.  
Example: `console.log('Hello'.length)`  

The . is another operator. It's called the `dot operator`  

### Methods

**methods** - actions that can be performed. Methods can be used, or called, by appending an instance with:  

- a period (dot operator)
- the name of the method
- opening and closing parentheses

Popular string methods include `.toUpperCase()` and `.startsWith()`, and `trim()`.  

### Built-in Objects

There are objects, such as console, built in to JavaScript. The Math object is one example of another built in object.  
`.random()` is a method from the Math object.  

### Variables

**variable** - a container in a computer's memory for a value.  
Variables provide a way of labeling data with a descriptive name, so programs can be understood more clearly.  
In short, variables label and store data in memory.  

**var** - a JavaScript keyword that creates (or declares) a new variable.  
Variable names cannot start with a number, are case sensitive, cannot be a JavaScript keyword, and should be written in camelCase.  

`=` is the assignment operator. It assigns a value (or initializes) to the variable name.  

**let** - a JavaScript keyword signaling the variable can be reassigned a different value.  

We can declare a variable without assigning it a value. In these cases, the variable is automatically initialized with a value of undefined.  

**const** - a JavaScript keyword signaling the variable *cannot* be reassigned a different value.  

- If you try to reassign a `const` variable, you'll get a TypeError.  

`const` variables *must* be assigned a value when declared.  

- If you try to declare a `const` variable without a value, you'll get a SyntaxError.  

### Mathematical Assignment Operators

We can use variables and math operators to calculate new values and assign them to a variable.  
`-=`, `*=`, and `/=` are operators that can shorten code from the longhand way of reassigning variables.  

### Increment and Decrement Operator

Mathematical assignment operators also include the *increment operator* (++) and *decrement operator* (--).  
The increment operator will increase the value of the variable by 1. The decrement operator will decrease the value of the variable by 1.  

### String Concatenation with Variables

The `+` operator can be used to combine two string values, even if they are stored in variables.  

### String Interpolation

In JavaScript we can insert, or *interpolate*, variables into strings using *template literals*.  
A template literal is wrapped in back ticks (``).  
Inside the template literal, there is a placeholder, `${variable}`. The value of `variable` is inserted into the template literal.  

Example:  

```javascript
var myName = 'Greg';
var myCity = 'Bozeman';
console.log(`My name is ${myName}. My favorite city is ${myCity}.`);
```

### typeof Operator

It can be useful to keep track of the data types of the variables in your program. If you need to check the data type of a variable’s value, you can use the typeof operator.  
The typeof operator checks the value to its right and returns, or passes back, a string of the data type.  

Example:  

```javascript
const foo = 'bar';
console.log(typeof foo); // Output: string
```

## Conditional Statements

A conditional statement checks a specific condition or conditions and performs a task based on the condition(s).  

### If Statement

**if** - a JavaScript keyword followed by a set of parentheses (`()`) in which the condition will be stated. The condition is followed by a *code block* or *block statement* indicated by a set of curly braces(`{}`) to carry out instructions based on the condition given.  

### If Else Statements

**else** - a JavaScript keyword paired with an if statement to handle situations where the if condition is not true.  

In many cases, you will want to evaluate a condition and perform some action if the condition is not met (or evaluates to false).  
In these situations we can add and `else` statement to run a block of code.  
An `else` statement must be paired with an if statement, and together they are referred to as an if...else statement.  

#### Else If

**else if** - a JavaScript keyword used in a conditional statement when more than one condition is to be evaluated.  
The `else if` statement allows for more than two possible outcomes.  

### Comparison Operators

When writing conditional statements, sometimes we need to use different types of operators to compare values. These operators are called comparison operators.  

The following are a few comparison operators and their syntax:  

- Less than: `<`
- Greater than: `>`
- Less than or equal to: `<=`
- Greater than or equal to: `>=`
- Is equal to (*identity operator*): `===`
- Is not equal to: `!==`

Comparison operators compare the value on the left with the value on the right.

All comparison statements evaluate to either true or false and are made up of:  

- Two values that will be compared.
- An operator that separates the values and compares them accordingly (>, <, <=,>=,===,!==)

### Logical Operators

In JavaScript, there are operators that work with boolean values known as logical operators. We can use logical operators to add more sophisticated logic to our conditionals. There are three logical operators:  

- and operator (&&)
- or operator (||)
- not operator, otherwise known as the bang operator (!)

When we use the `&&` operator, we are checking that two things are true. Both things must be true for the overall statement to evaluate to true.  
When using the `||` operator, only one of the conditions must evaluate to true for the overall statement to evaluate to true.  
The `!` not operator reverses, or negates, the value of a boolean. Essentially, the `!` operator will either take a true value and pass back false, or it will take a false value and pass back true.  

Logical operators are often used in conditional statements to add another layer of logic to our code.  

### Truthy and Falsy

**truthy** - evaluates to a non-falsy value.  
**falsy** - values the evaluate to `0`, empty strings (`""` or `''`), `null` (represents when there is no value at all), `undefined` (represents when a declared variable lacks a value), and `NaN` (not a number).  

### Ternary Operator

A ternary operator can be used to simplify an if...else statement using a question mark (`?`) with the two expressions separated by a colon (`:`).  
If the first condition evaluates to true, the first expression is executed. If the first condition evaluates to false, the second expression is executed.  

### Switch Statements

**switch statement** - provides an alternate syntax that is easier to read and write when many conditions are being evaluates (rather than writing many else if statements).  

The `switch` keyword initiates the statement and is followed by ( ... ), which contains the value that each case will compare.  

## Functions

### What are Functions?

We often use code to perform a specific task multiple times. Instead of rewriting the same code over and over, we can group a block of code together and associate it with one task, then we can reuse that block of code whenever we need to perform the task again. We achieve this by creating a function.  
**function** - a reusable block of code that groups together a sequence of statements to perform a specific task.  

### Function Declarations

A function declaration is a way to create a function in JavaScript. A function declaration binds a function to a name, or an *identifier*.  
A function declaration consists of:  

- the `function` keyword
- the name (identifier) of the function followed by parentheses.
- A function body, or the block of statements required to perform a specific task, enclosed in curly braces (`{}`)  

### Calling a Function

The code inside the body of a function is only executed when the function is called.  
To call a function, type the function name (identifier) followed by parenthesis.  

Example: `functionIdentifier();`  

### Parameters and Arguments

Functions can take inputs and use the inputs to perform a task. When declaring a function, we can specify its *parameters*. Parameters allow functions to accept input(s) and perform a task using the input(s). Parameters are placeholders for information that will be passed to the function when it is called.  

**arguments** - values that are passed to a function when it is called.  
Arguments can be passed to the function as values or variables.  

### Default Parameters

**default parameters** - allow parameters to have a predetermined value in case there is no argument passed into the function or if the argument is undefined when called.  

By using a default parameter, we account for situations when an argument isn’t passed into a function that is expecting an argument.  

### Return

**return** - a JavaScript keyword that allows for capturing the output of a function and passing back the information.  

The return keyword is powerful because it allows functions to produce an output. We can then save the output to a variable for later use.  

### Helper Functions

You can return the value of a function inside another function.  
**helper functions** - a function called within another function.  

### Function Expressions

A function expression is another way to define a function. In a function expression, the function name is usually omitted. A function with no name is called an anonymous function. A function expression is often stored in a variable in order to refer to it.  

### Arrow Functions

**arrow functions** - remove the need to type out the `function` keyword every time you create a function.  
Instead, you first include the parameters inside the ( ) and then add an arrow => that points to the function body surrounded in `{}`.  
Also known as “fat arrow” () => notation.  

Example:  

```javascript
const rectangleArea = (width, height) => {
  let area = width * height;
  return area;
};
```

### Concise Body Arrow Functions

Functions that take only a single parameter do not need that parameter to be enclosed in parentheses. However, if a function takes zero or multiple parameters, parentheses are required.  

Zero Parameters - `const functionName = () => {};`  
One Parameter - `const functionName = paramOne => {};`  
Two or More Parameters - `const functionName = (paramOne, paramTwo) => {};`  

A function body composed of a single-line block does not need curly braces. Without the curly braces, whatever that line evaluates will be automatically returned. The contents of the block should immediately follow the arrow => and the return keyword can be removed. This is referred to as *implicit return*.  

Single Line Block - `const sumNumbers = number => number + number;`  
Multi Line Block:  

```javascript
const sumNumbers = number => {
    const sum = number + number;
    return sum;
};
```

## Scope

### Blocks and Scope

A block is code inside a set of curly braces.  

### Global Scope

Scope is the context in which our variables are declared. We think about scope in relation to blocks because variables can exist either outside of or within these blocks.  

**global variables** - variables declared outside of blocks. These variables have a global scope.  

### Block Scope

**local variables** - variables only accessible within a block of code. Also known as block scope variables.  

### Scope Pollution

Scope pollution is when we have too many global variables that exist in the global namespace, or when we reuse variables across different scopes.  
Scope pollution makes it difficult to keep track of our different variables and sets us up for potential accidents. For example, globally scoped variables can collide with other variables that are more locally scoped, causing unexpected behavior.  

### Scope Review

**scope** - the idea in programming that some variables are accessible/inaccessible from other parts of the program.  
**blocks** - statements that exist within curly braces {}.
**global scope** - refers to the context within which variables are accessible to every part of the program.  
**global variables** - variables that exist within global scope.  
**block scope** refers to the context within which variables that are accessible only within the block they are defined.  
**local variables** - variables that exist within block scope.  
**global namespace** - the space in our code that contains globally scoped information.  
**scope pollution** - when too many variables exist in a namespace or variable names are reused.  

## Arrays

An array is a means of storing data in a list like structure.  
Each content item inside an array is called an *element*.  

### Accessing Elements

**index** - an element in an array's numbered position.  
Individual elements (items) can be accessed using their index.  
Arrays in JavaScript are zero-indexed, meaning the positions start counting from 0.  

### Update Elements

Once you have access to an element in an array, you can update its value.  

### Arrays with Let and Const

You can declare variables with both the let and const keywords. Variables declared with let can be reassigned.  
Variables declared with the const keyword cannot be reassigned. However, elements in an array declared with const can be changed, but we cannot reassign a new array or a different value.

### Helpful Array Methods

`.length`  
`.push()`  
`.pop()`  

[More Array Methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array#static_methods)

### Nested Arrays

Arrays can store other arrays. These are known as nested arrays.  
To access the nested arrays we can use bracket notation with the index value.  

## Loops

A loop is a tool in programming that repeats a set of instructions until a specified condition, called a *stopping condition*, is reached.  

**iterate** - to repeat  

### For Loops

A for loop contains three expressions separated by ; inside the parentheses:

1. an initialization starts the loop and can also be used to declare the iterator variable.
1. a stopping condition is the condition that the iterator variable is evaluated against— if the condition evaluates to true the code block will run, and if it evaluates to false the code will stop.
1. an iteration statement is used to update the iterator variable on each loop.

### Looping through an Array

To loop through each element in an array, a for loop should use the array’s .length property in its condition.  

### While Loop

The while loop starts with the **while** keyword followed by a *stopping condition*, or *test condition*. This will be evaluated before each round of the loop. While the condition evaluates to true, the block will continue to run. Once it evaluates to false the loop will stop.  

### Do...While Statements

Do While statements are used when you want a piece of code to be run at least one time and then keep doing it until a specified condition is no longer met.  

### break Keyword

The break keyword allows programs to “break” out of the loop from within the loop’s block.  

## Higher-Order Functions

**higher-order functions** - functions that accept other functions as arguments and/or return functions as output.  
Using more abstraction in code allows us to write more modular code, which is easier to read and debug.  

### Functions as Data

We can assign functions to alias names (variables) in order to shorten them when calling them.  
Example:  

```javascript
const alias = superVeryLongFunctionName;
alias(); // shorter function call.
```

In JavaScript, functions are first class objects. This means that JavaScript functions can have properties and methods.

### Functions as Parameters

**invoking a function** - means to directly call a function to run it.  
**callback function** - a function passed as an argument into another function.  
Parameters can take in functions the same as other types of data in JavaScript.  
When we pass a function in as an argument to another function, **we don’t invoke it**. Invoking the function would evaluate to the return value of that function call.  
With *callbacks*, we pass in the function itself by typing the function name **without** the parentheses (that would evaluate to the result of calling the function).  

## Iterators

**iterate** - loop through.  
**iteration methods** - built-in JavaScript array methods that help to iterate.  

Helpful iterator methods:  

`.forEach()`

- the `.forEach()` method executes the same code on each element of an array.  
- `.forEach()` takes an argument of callback function.  
- `.forEach()` loops through the array and executes the callback function for each element. During each execution, the current element is passed as an argument to the callback function.  
- The return value for `.forEach()` will always be `undefined`.  

`.map()`  

- When `.map()` is called on an array, it takes a callback function argument and returns a new array.
- `.map()` works in a similar manner to `.forEach()` — the major difference is `.map()` returns a new array.

`.filter()`

- `.filter()` also returns a new array, but only after filtering out certain elements from the original array.  
- The callback function for the `.filter()` method should return `true` or `false` depending on the element passed to it. Elements causing the callback function to return `true` are added to the new array.  

`.findIndex()`  

- `.findIndex()` is used to find the location of an element in an array. It will return the index of the first element that evaluates to true in the callback function.  

`.reduce()`  

- `.reduce()` returns a single value after iterating through the elements of an array, thereby reducing the array.

`.some()`  

`.every()`

## Objects

Objects are the basic structure that permeate nearly every aspect of JavaScript programming.  
Objects are the seventh fundamental data type of JavaScript.  
At their core, JavaScript objects are containers storing related data and functionality, but that simple task is extremely powerful in practice.  

### Creating Object Literals

Objects can be assigned to variables just like any JavaScript type. Curly braces `{}` are used to designate an object literal.  
Example: `let object = {}; //object is an empty object`  

Objects are filled with unordered data. This data is organized into key-value pairs. A key is like a variable name that points to a location in memory that holds a value.  
A key-value pair is made by writing the key's name, or *identifier*, followed by a colon and then the value. Example: `key: value`  
Each key-value pair in an object literal is separated with a comma.  

Keys are strings, but if no special characters are present, JavaScript allows us to omit quotation marks around it.  

### Accessing Properties

Dot Notation can be used to access items in an object.  
Example:  

```javascript
let object = {
    key: 'value',
    color: 'green'
};

object.key; // returns value
object.color; // returns green
```

If a property that does not exist is attempted to be accessed, `undefined` will be returned.  

### Bracket Notation

Another way to access a key's value is to use bracket notation `[ ]`  
To use bracket notation to access an object's property, pass in the property name as a sting.  
Example: `object['key'];`  

Using bracket notation is **required** when accessing keys that have numbers, spaces, or special characters in them. Without bracket notation in these situations, the code will throw an error.  

### Property Assignment

Objects are mutable, meaning we can update or change them.  
Either dot or bracket notation can be used along with the assignment operator (`=`) to add new key-value pairs to an object or change an existing property.  

One of two things can happen with property assignment:  

- If the property already exists on the object, whatever value it held before will be replaced with the newly assigned value.
- If there was no property with that name, a new property will be added to the object.

It's important to remember we can't reassign an object declared with `const`, but we can still mutate it, meaning we can add new properties and change properties within the object.  

To delete a property from an object, use the `delete` operator.  
Example: `delete object.key; //removes the key property`  

### Object Methods

When the data stored in an object is a function, that is called a *method*. A property is what an object *has*. A method is what an object *does*.

### Nested Objects

In application code, objects are often nested. An object may have another object as a property, which in turn could have a property that's an array of even more objects.  

Operators can be chained to access nested properties.  

### Pass By Reference

Objects are passed by reference. This means when we pass a variable assigned to an object into a function as argument, the computer interprets the parameter name as pointing to the space in memory holding that object. As a result, functions which change object properties actually mutate the object permanently (even when the object is assigned to a const variable).

### Looping Through Objects

Loops are programming tools that repeat a block of code until a condition is met.  
JavaScript gives us an alternative solution for iterating through objects. The `for...in` syntax.  
`for...in` will execute a given block of code for each property in an object.  

## Advanced Objects

Objects in JavaScript are containers that store data and functionality.  

### The this Keyword

The `this` keyword allows for access to properties outside of a method's scope in an object. `this` references the *calling object* which provides access to the calling object's properties.  

In JavaScript, `this` will always refer to an object.  

Avoid using arrow functions when using `this` in a method.  

### Privacy

Accessing and updating properties is fundamental in working with objects. However, there are cases in which we don’t want other code accessing and updating an object’s properties. When discussing privacy in objects, we define it as the idea that only certain properties should be mutable or able to change in value.

Certain languages have privacy built-in for objects, but JavaScript does not have this feature. Rather, JavaScript developers follow naming conventions that signal to other developers how to interact with a property. One common convention is to place an underscore _ before the name of a property to mean that the property should not be altered.

*type-coercion* - the process of converting value from one type to another.  

### Getters

Getters are methods that get and return the internal properties of an object.  
Getter can perform an action on the data when getting a property.  
Getters can return different values using conditionals.  
In a getter, we can access the properties of the calling object using `this`.  
The functionality of our code is easier for other developers to understand.  

When using getter and setter methods is that properties cannot share the same name as the getter/setter function. If this is done, calling the method will result in an infinite call stack error. One workaround is to add an underscore before the property name.  

[**typeof**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/typeof) - returns a string indicating the type of the unevaluated operand. Can also be used to check the type of value in a conditional statement.  
Example:  

```javascript
if (typeof this._variable === 'number') {
    return 'string';
```

### Setters

Along with getter methods, we can also create setter methods which reassign values of existing properties within an object.  

Setter methods do not need to be called with a set of parentheses. Syntactically, it looks like we’re reassigning the value of a property.  

Like getter methods, there are similar advantages to using setter methods that include checking input, performing actions on properties, and displaying a clear intention for how the object is supposed to be used. Nonetheless, even with a setter method, it is still possible to directly reassign properties.  

### Factory Functions

**factory functions** - a function that returns an object and can be reused to create many instances of an object quickly.  

### Property Value Shorthand

**property value shorthand** - a destructuring technique to save keystrokes. Property assignments don't require to be fully defined.  
Example:  

```javascript
const object = (var1, var2) => {
  return { 
    var1,
    var2 
  }
};
```

### Destructured Assignment

A common desire in JavaScript is to assign object properties to variables.  
**destructured assignment** - the creation of a variable in curly braces `{}` and assigning it to an object.  
Example:  

Traditional method:  

```javascript
const objectProperty = object.ObjectProperty; 
console.log(objectProperty);
```

Destructured assignment:  

```javascript
const { objectProperty } = object; 
console.log(objectProperty);
```

### Built-in Object Methods

JavaScript has many built in methods available.  
[JavaScript Object Method Documentation - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object#Methods)  

## Classes

JavaScript is an object-oriented programming (OOP) language. Classes are tools that developers use to quickly produce similar objects.  
Classes are a great way to reduce duplicate code and debugging time.  
For styling, class names are capitalized and written in CamelCase format.  

### Constructor

The constructor is a method used to create a new instance of a class.  
JavaScript will invoke the `constructor()` every time a new instance of a class is created.  
Inside the constructor method, the `this` keyword is used to refer to an instance of that class.  
Example:  

```javascript
class ClassName {
    constructor() {
        this.item = item;
    }
}
```

### Instance

An instance is an object that contains the property names and methods of a class, but with unique property values.  

### Class Methods

Class methods and getter syntax is the same as it is for objects **except you cannot include commas between methods.**  

### Method Calls

The syntax for calling methods and getters on an instance is the same as calling them on an object. Append the instance with a period, then add the property or method name.  
Methods must also include opening and closing parentheses.  

### Inheritance

When multiple classes share properties or methods, they become candidates for *inheritance*.  
**inheritance** - the ability to access object properties from another object.  

With inheritance, you can create a parent class (also known as a superclass) with properties and methods that multiple child classes (also known as subclasses) share.  

Syntax for subclass to inherit from superclass:  

```javascript
class SubClass extends SuperClass {
    constructor(param1, param2, paramN){
        super(param);
    }
}
```  

**extends** - JavaScript keyword which allows methods of the superclass to be available to the subclass.  
**super** - JavaScript keyword which calls the constructor of the parent class.  

In a constructor, you must always call the `super` method before you can use the `this` keyword. If it is not, JavaScript will throw a reference error.  
To avoid this, it is best practice to call `super` on the first line of the subclass constructor.  

### Static Methods

**static methods** - methods that aren't available in individual instances, but that can be called directly from the class.  

Using the `static` keyword makes a method only accessible when appending it to its native class.  
If calling a static method is attempted by a subclass or any instance of a class, JavaScript will throw a TypeError.  

## Browser Compatibility

Two important tools for addressing browser compatibility issues.  
[caniuse.com](https://caniuse.com/)  
[Babel](https://babeljs.io/)  

**transpilation** - the process of converting one programming language to another.  

### Babel

Babel is a JavaScript library that transpiles ES6 JavaScript to ES5.  
To install Babel, run `npm install babel-cli` and then `npm install babel-preset-env`  

### npm init

Developers use npm to access and manage Node packages. Node packages are directories that contain JavaScript code written by other developers. These packages can be used to reduce duplication of work and avoid bugs.  
The `npm init` command creates a **package.json** file in the root directory.  
A package.json file contains information about the current JavaScript project. Some of this information includes:  

- metadata - such as project title, description, authors, and more.
- A list of node packages required for the project
- key-value pairs for command line scripts

### Install Node Packages

`npm install` is used to install new Node packages manually. The `install` command also creates a folder called node_modules and copies the package files to it. The `install` command installs all of the dependencies for the given package.  

To install babel, run: `babel-cli` and `babel-preset-env`  

The .babelrc file specifies the version of the JavaScript source code.  

It is possible to build scripts in the scripts block of the package.json file.  

## Modules

**modules** - reusable pieces of code that can be exported fro one program and imported for use in another program.  

Modules are useful for many reasons. By separating code with similar logic into files (called modules) we can:

- find, fix, and debug code more easily
- reuse and recycle defined logic in different parts of our application
- keep information private and protected from other modules
- prevent pollution of the global namespace and potential naming collisions, by cautiously selecting variables and behavior we load into a program

There are two ways to implement modules in JavaScript.  

- `module.exports` and `require()` syntax
- `import`/`export` syntax

### module.exports

Every JavaScript file run in Node has a local module object with an exports property used to define what should be exported from the file.
Syntax for exporting a module.  
`module.exports = exportedObject`  

### require()

In Node.js the `require()` function is used to import modules.  
`require()` takes a file path pointing to the original module file as the argument.  
Example: `require('/path/to/filename.js');`

The pattern to import a module is:

1. Import the module with require() and assign it to a local variable.  
    - Example: `const request = require('request');`
1. Use the module and its properties within a program.

### export default

Node.js supports `require()`/`module.exports`, but as of ES6, JavaScript supports a new, more readable, and flexible syntax for exporting modules. These are usually broken down into one of two techniques, *default export* and *named exports*.  

**export default** - uses the JavaScript `export` statement to export JavaScript objects, functions, and primitive data types.  
Example:  

```javascript
let Object = {};
export default Object;
```

In ES6, `export default` is used in place of `module.exports`. Node.js doesn't support `export default` by default, so `module.export` is still usually used for Node.js.  

### import

ES6 module syntax introduces the `import` keyword for importing objects. The `import` keyword begins the import statement and `from` specifies where to load the module from.  
Example: `import Object from '/path/to/object/location';`  

### Named Exports

ES6 introduced a second common approach to export modules. `named exports` allow us to export data through the use of variables.  
When using named exports, properties are not set on an object. Each export is stored in its own variable. The `export` keyword is the prefix.  
Example:  `export {variable, function, object, etc};`  

### Named Imports

To import objects stored in a variable, the `import` keyword is used and include the variables in a set of curly braces `{}`.  
Syntax example: `import {variable, function, object, etc} from '/path/to/object/location';`  

### Export Named Exports

Named exports are distinct in that they can be exported as soon as they are declared by placing the keyword `export` in front of variable declarations.  
Example: `export let variable = '';` or `export function functionName() {};`  

The `export` keyword allows us to export objects upon declaration. With this method, an `export` statement is no longer needed at the bottom of the file.  

### Import Named Imports

To import variables that are declared, simply use the original syntax that describes the variable name. Exporting upon declaration (see section directly above) does not have an impact on how variables are imported.  
Example: `import {variable, function, object, etc} from 'path/to/object/location';`  

### Export as

Named exports offer a way to change the name of variables we export or import. This is done with the `as` keyword.  
Example: `export {variable as variable1, function as newFunction, longObject as shortObj};`  

### Import as

To import named export aliases with the `as` keyword, add the aliased variables to the import statement.  
Example: `import {variable1, newFunction, shortObj} from 'path/to/object/location';`  

Another way of using aliases is to import the entire module as an alias.  
Example: `import * as AliasName from 'path/to/object/location';`  

Reference these objects with the alias name followed by the object.  
Example: `AliasName.variable1;` or `AliasName.newFunction();`  

### Combining Export Statements

It is possible to use named exports and default exports together.  
The `export` keyword is used to export the named exports at the bottom of the file. The `export default` keyword is then used for any objects desired to be exported as well.  

It's best to avoid combining two methods of exporting, but it is useful on occasion.  

### Combining Import Statements

The `import` keyword is used to import variables in various methods.  

## Promises

**asynchronous operation** - one that allows the computer to “move on” to other tasks while waiting for the asynchronous operation to complete.  

Web development makes use of asynchronous operations. Operations like making a network request or querying a database can be time-consuming, but JavaScript allows us to execute other tasks while awaiting their completion.

**promise** - objects that represent the eventual outcome of an asynchronous operation.  

A `Promise` object can be in one of three states:  

- Pending - the initial state. The operation has not completed yet.  
- Fulfilled - the operation has completed successfully and the promise now has a *resolved value*.
- Rejected - The operation has failed and the promise has a reason for the failure. This reason is usually an `Error` of some kind.  

A promise is referred to as *settled* if it is no longer pending. It is either fulfilled or rejected.  
All promises eventually settle, enabling logic to be written for what to do if the promise fulfills or if it rejects.  

### Constructing a Promise Object

To create a new `Promise` object, use the `new` keyword and the `Promise` constructor method.  
The `Promise` constructor method takes a function parameter called the `executor function` which runs automatically when the constructor is called. The executor function typically starts an asynchronous operation and dictates how the promise should be settled.  

The executor function has two function parameters, `resolve()` and `reject()`.  
These functions are not defined by the programmer. When the `Promise` constructor runs, JavaScript will pass its own resolve() and reject() functions into the executor function.  

- `resolve` is a function with one argument. Under the hood, if invoked, resolve() will change the promise’s status from pending to fulfilled, and the promise’s resolved value will be set to the argument passed into resolve().
- `reject` is a function that takes a reason or error as an argument. Under the hood, if invoked, reject() will change the promise’s status from pending to rejected, and the promise’s rejection reason will be set to the argument passed into reject().

### The Node setTimeout() Function

Knowing how to construct a promise is useful, but knowing how to consume (or use) promises is a more common use case. Handling `Promise` objects returned to you as the result of an asynchronous operation is more common than constructing new promises. These promises will start off pending but settle eventually.  

The `setTimeout()` function has two parameters: a callback function and a delay in milliseconds.  
Example: `setTimeout(callbackFunction, 1000)`  

### Consuming Promises

Promise objects come with a `.then()` method that instructs the computer what do after a promise is settled (resolved or rejected).  

`.then()` is a higher-order function. It takes two callback functions as arguments, commonly referred to as handlers. When the promise settles, the appropriate handler will be invoked with the settled value.  

- The first handler, sometimes called `onFulfilled`, is a **success handler**, and it should contain the logic for the promise resolving.
- The second handler, sometimes called `onRejected`, is a **failure handler**, and it should contain the logic for the promise rejecting.

`.then()` can be invoked with one, both, or neither handler, allowing flexibility but also potentially difficult debugging.  
One important feature of `.then()` is it always returns a promise.  

### Success and Failure Callback Functions

With typical promise consumption, it isn't known whether a promise will resolve or reject, so  providing the logic for either case is needed. To do this, pass both a success callback and a failure callback to `.then()`.  
Example:  

```javascript
let promise = new Promise((resolve, reject) => {
  let num = Math.random();
  if (num < .5 ){
    resolve('Resolved');
  } else {
    reject('Rejected');
  }
});
 
const handleSuccess = (resolvedValue) => {
  console.log(resolvedValue);
};
 
const handleFailure = (rejectionReason) => {
  console.log(rejectionReason);
};
 
promise.then(handleSuccess, handleFailure);
```

The success callback is sometimes called the “success handler function” or the onFulfilled function. The failure callback is sometimes called the “failure handler function” or the onRejected function.  

### Using catch() with Promise

To write cleaner code follow a principle called **separation of concerns**. Separation of concerns means organizing code into distinct sections each handling a specific task. It enables developers to quickly navigate code and know where to look if something isn’t working.  

`.catch()` is a different promise function that takes only one argument, onRejected. It is possible to chain together `.then()` functions with success and failure headers, but `.catch()` makes code more readable.  
Example:  

```javascript
promise
    .then((resolvedValue) => {
        console.log(resolvedValue);
    })
    .catch((rejectedValue) => {
        console.log(rejectionReason);
    });
```

### Chaining Multiple Promises

A common pattern seen with asynchronous programming is multiple operations which depend on each other to execute or that must be executed in a certain order. One request may be made to a database and use the data returned to make another request and so on.  

**composition** - the process of chaining promises together.  
Promises are designed with composition in mind.  

### Avoiding Common Mistakes

**Mistake 1** - Nesting promises instead of chaining them.  
**Mistake 2** - Forgetting to return a promise.  

### Using Promise.all()

Promise composition is a great way to handle situations where asynchronous operations depend on each other or execution order matters. But in situations when dealing with multiple promises and order is not important, `Promise.all()` can be used to maximize efficiency.  

`Promise.all()` accepts an array of promises as its argument and returns a single promise. That single promise will settle in one of two ways:

- If every promise in the argument array resolves, the single promise returned from `Promise.all()` will resolve with an array containing the resolve value from each promise in the argument array.
- If any promise from the argument array rejects, the single promise returned from `Promise.all()` will immediately reject with the reason that promise rejected. This behavior is sometimes referred to as failing fast.

## Async-Await

**asynchronous actions** - actions that can be waited on while moving on to other tasks.  

Often in web development, there is a need to handle asynchronous actions. Requests are made to networks, databases, or any number of similar operations.  
JavaScript is non-blocking: instead of stopping the execution of code while it waits, JavaScript uses an event-loop which allows it to efficiently execute other tasks while it awaits the completion of these asynchronous actions.  

### The async Keyword

The `async` keyword is used to write functions that handle asynchronous actions. Asynchronous logic is wrapped inside a function prepended with the `async` keyword. Then, the function is invoked.  

`async` functions always return a promise. This means traditional promise syntax, like `.then()` and `.catch()` can be used. An `async` function will return in one of three ways:  

- If there's nothing returned from the function, it will return a promise with a resolved value of `undefined`.  
- If there's a non-promise value returned from the function, it will return a promise resolved to that value.  
- If a promise is returned from the function, it will return that promise.

### The await Operator

The `async` keyword is almost always used with the additional keyword `await` inside the function body.  
The `await` keyword can only be used inside an `async` function. `await` is an operator: it returns the resolved value of a promise.  
Since promises resolve in an indeterminate amount of time, `await` halts, or pauses, the execution of an async function until a given promise is resolved.  

### Writing async Functions

Don't forget the `await` keyword.  

### Handling Dependent Promises

The true beauty of `async...await` is when a series of asynchronous actions depend on one another.  

Though using the `async...await` syntax can save typing, the length reduction isn’t the main point.  
Given the two versions of the function, the `async...await` version more closely resembles synchronous code, which helps developers maintain and debug their code.  

### Handling Errors

When `.catch()` is used with a long promise chain, there is no indication of where in the chain the error is thrown. This can make debugging challenging.  
With `async...await`, `try...catch` statements are used for error handling. By using this syntax, not only are we able to handle errors in the same way we do synchronous code, but we can also catch both synchronous and asynchronous errors. This makes debugging easier.  

### Handling Independent Promises

`await` halts the execution of an `async` function. This allows for writing synchronous-style code to handle dependent promises.  
If an `async` function contains multiple promises which are not dependent on the results of other promises to execute, the `waiting()` and `concurrent()` functions can be used.  

In the `waiting()` function, the function is paused until the first promise resolves, then the second promise is constructed. This can continue for as many times as needed.  

In the `concurrent()` function, both promises are constructed without using the `await` keyword. Each promise waits for their resolutions before returning them.  
With the `concurrent()` function, promises’ asynchronous operations can be run simultaneously. If possible, starting each asynchronous operation as soon as possible is desirable. Within async functions we should still take advantage of *concurrency* - the ability to perform asynchronous actions at the same time.  

### Await Promise.all()

Another way to take advantage of *concurrency* when working with multiple promises that can be executed simultaneously is to `await` a `Promise.all()`.  
You can pass an array of promises as the argument to `Promise.all()`, and it will return a single promise. This promise will resolve when all of the promises in the argument array have resolved.  
This promise’s resolve value will be an array containing the resolved values of each promise from the argument array.  

`Promise.all()` allows us to take advantage of asynchronicity. `Promise.all()` also has the benefit of *failing fast*, meaning it won’t wait for the rest of the asynchronous actions to complete once any one has rejected.  
As soon as the first promise in the array rejects, the promise returned from `Promise.all()` will reject with that reason.  

## Requests

HTTP Requests are triggered upon submitting information from a web page.  
There are many types of HTTP requests, but the four most commonly used types of HTTP requests are GET, POST, PUT, and DELETE.  

[HTTP Request Methods](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods)  

With a GET request, we’re retrieving, or getting, information from some source (usually a website). For a POST request, we’re posting information to a source that will process the information and send it back.  

[JavaScript XHR (XMLHTTPRequest) Object](https://developer.mozilla.org/en-US/docs/Web/API/XMLHttpRequest)  

### HTTP Requests

One of JavaScript's greatest assets is its non-blocking properties, or that it is an *asynchronous language*.  
Web sites take advantage of these non-blocking properties to provide a better user-experience.  
An example of this may be, a site’s code is written so users don’t have to wait for a giant image to load before being allowed to read the actual article. Rather, the text is rendered first and then the image can load in the background.  

JavaScript uses an *event loop* to handle asynchronous function calls. When a program is run, function calls are made and added to a stack. Functions that make requests needing to wait for a server response get sent to a separate queue. Once the original stack of functions is cleared, the waiting queue functions are executed.  

Web developers use the event loop to create a smoother browsing experience by deciding when to call functions and how to handle asynchronous events.  

[Event Loop Documentation - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/EventLoop)  

### XHR GET Requests

Asynchronous JavaScript and XML (AJAX) enables requests to be made after the initial page load.  
Initially, AJAX was used only for XML formatted data, but now it can be used to make requests that have many different formats.  

[XML Documentation - MDN](https://developer.mozilla.org/en-US/docs/Web/XML/XML_introduction)  

Similarly, the XMLHTTPRequest (XHR) API can be used to make many kinds of requests and supports other forms of data.  

**json** - JavaScript Object Notation.  

**query string** - a string containing additional information to be sent with a request.  
A query string is separated from the URL using a `?` character. After `?`, you can then create a parameter which is a key value pair joined by a `=`.  
Example: `https://api.site.com/apiaddress?key=value`  

If you want to add an additional parameter you will have to use the & character to separate your parameters.  

### XHR POST Requests

The major difference between a GET request and POST request is a POST request requires additional information to be sent through the request. This additional information is sent in the body of the post request.  

### Introduction to Requests with ES6

To make asynchronous event handling easier, *promises* were introduced in JavaScript in ES6.  

[Promise Documentation - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)  

**promise** - an object that handles asynchronous data.  

A promise has three states:

- pending - when a promise is created or waiting for data.
- fulfilled - the asynchronous operation was handled successfully.
- rejected - the asynchronous operation was unsuccessful.

The great thing about promises is that once a promise is fulfilled or rejected, you can chain an additional method to the original promise.  

`fetch()` - uses promises to handle requests.  

### fetch() GET Requests

[Fetch API Documentation - MDN](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)  

The `fetch()` function:  

- Creates a request object that contains relevant information that an API needs.  
- Sends that request object to the API endpoint provided.  
- Returns a promise that ultimately resolves to a response object, which contains the status of the promise with information the API sent back.  

### fetch() POST Requests

The initial `fetch()` POST call takes two arguments: an endpoint and an object containing information needed for the POST request.  
