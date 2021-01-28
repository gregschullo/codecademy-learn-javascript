---
id: learn-javascript
title: Learn Javascript
---

[Codecademy Course - Learn JavaScript](https://www.codecademy.com/learn/introduction-to-javascript)  

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
