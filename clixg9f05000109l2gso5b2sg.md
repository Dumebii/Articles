---
title: "Introduction to Javascript"
seoTitle: "Javascript fundamentals// beginner javascript// javascript variables"
seoDescription: "Learn Javascript Javascript fundamentals Loops in javascript  conditional statements in javascript  scope in javascript   conditionals naming conventions"
datePublished: Thu Jun 15 2023 18:03:45 GMT+0000 (Coordinated Universal Time)
cuid: clixg9f05000109l2gso5b2sg
slug: learn-front-end-web-development-in-12-days-beginner-javascript
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1686839909923/80035499-0721-475f-be66-8f4b88959ab2.png
tags: tutorial, javascript, web-development, beginners, conditional-statement

---

Hello and welcome!! 🤩🤩🤩

Today we will be starting our Javascript class.

Javascript is a vast topic. Javascript has been adapted to various aspects of technology and programming, including AI, web development, and others.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1686839855942/84d7fe98-4f6c-4eb1-8d7b-0b2d0c6c1154.jpeg align="center")

In this tutorial, I will explain some important key concepts to note as you go on your Javascript journey. However, some concepts I will be demonstrating with a solved example.

## Introduction

👉🏾 Javascript is the world's most popular programming language.

👉🏾 Javascript is the programming language of the Web.

👉🏾 JavaScript is easy to learn. 😏

## Javascript Keywords

***In computer programming, keywords are predefined words in a programming language with a specific use. Additionally, we use them to define the structure and flow of a program. Furthermore, they specify the operations that the program should perform.***

In javascript, there are keywords like `const`, `var`, `catch`, `await`, `typeOf`, `static`, `protected`, `goTo`, `let` amongst others.

## Variable declaration

Think of a variable as an empty container in which you want to store a product. Let me paint a scenario: you are moving out of your house, and have gathered a lot of moving boxes to contain your belongings. You start in the living room, pick up a box, label it "living room", and put all the living room items in it. You continue this process until you get to the garage. The boxes are variables, meaning they can contain any information or data. The labeling is called a variable name, and the items inside the box are the data stored in the variable.

`x = 'I am a stranger in this land.'`

In the above example; we see that `x` is the variable name, `I am a stranger in this land` is the information we are storing in a box `x` (which is our variable). `=` is a connector. Its function is to connect a variable name with the data to be stored in the variable.

## Data types in Javascript

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1686839413084/a7e660e9-4474-4620-b853-9799a1a62a77.jpeg align="center")

Data types define the various forms of data that we will be working with and storing in variables. There are five basic, or primitive, forms of data in Javascript. `Strings`, `integers`, `booleans`, `undefined`, and `null` are the five most fundamental forms of data. These are known as primitive data types. ***A single variable can only hold one kind of data.***

Let's go over each type of data and what it can be used for in more detail.

* **Strings** are collections of alphanumeric and symbol characters. This is how we'll save letters and words, such as addresses.
    
* **Numbers** are exactly how they sound. They are numbers, including integers and decimals. Numbers are frequently used by computers to execute mathematical operations, but they can also simply be a number, such as the number of ice cream flavors available at a given establishment.
    
* **Booleans** can only have two possible values. Both true and false. They represent any data that has only two states, such as a light switch. Either on or off.
    
* **The undefined data** type indicates that the variable was created but never assigned a value. It is nothing because no one has bothered to tell it what it should be worth.
    
* **Null** is similar to undefined in that it must be explicitly set. It also implies emptyness or nothingness, but it's because a developer commanded it to be that way.
    

## Naming conventions in javascript

When working in an organization, as a team, or individually, certain principles have to be followed or adhered to. This can vary depending on individual, team, or company standards.

* Variable names should have meaning, representing what data they are holding or where they are to be used.
    
* Variable names in JavaScript are conventionally written using the camelCase method. In the case of a compound word name, the first letter of the second word should be capitalized, while the others are in small letters.
    
* End every piece of code or code block with a semicolon `;` . Unlike in other languages with strict syntax rules, when writing Javascript code, semicolons are not added, it doesn't break the flow of the code. However, it is important to add these semicolons for readability.
    

*You can find more Javascript conventions* [*here.*](https://www.w3schools.com/js/js_conventions.asp)

## Scope in Javascript

Scope determines the accessibility (visibility) of variables. JavaScript has 3 types of scope:

* Block scope
    
* Function scope
    
* Global scope
    

**Block scope**: Before ES6 (2015), JavaScript had only **Global Scope** and **Function Scope**. ES6 introduced two important new JavaScript keywords: `let` and `const`. These two keywords provide **Block Scope** in JavaScript. Variables declared inside a `{ }` block cannot be accessed from outside the block.

```javascript
{
  let x = 2;
}
// x can NOT be used here
```

**Function scope**: JavaScript has function scope: Each function creates a new scope. Variables defined inside a function are not accessible (visible) from outside the function. Variables declared with `var`, `let` and `const` are quite similar when declared inside a function.

```javascript
function functionExample() {
  var variableName = "Volvo";   // Function Scope
};
```

**Global scope**: Variables declared **Globally** (outside any function) have Global Scope. Global variables can be accessed from anywhere in a JavaScript program. Variables declared with `var`, `let` and `const` are quite similar when declared outside a block.

```javascript
let x = 2;  // Global scope
```

## Javascript blocks

### Functions

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1686847971567/6714490d-4ab2-4481-8859-9c27ebdbdabf.png align="center")

A function is a block of reusable code written to perform a specific task. You can think of a function as a sub-program within the main program. A function consists of a set of `statements` but executes as a single unit. A function can be written like:

* ```javascript
        function sayHello() {
        	console.log("Hello world"); 
        };
        // sayHello()
    ```
    
    The code block above is the common syntax for writing a function in javascript. There is present the `function` keyword. The name of the function is followed by parentheses which can include parameters or be left blank, and a set of curly braces that encloses the entire function block. A set of instructions or *arguments* that are supposed to run once the function is called.
    
    Outside the function scope, we see, `sayHello()` this is a function call. Meaning, we are telling our computer to execute the commands within the function block.
    
* ```javascript
      function addNumbers(num1, num2) {
       console.log(num1 +num2) 
      };
      addNumbers(1, 2);
    ```
    
    The above is an example of a function with parameters. A function can contain many parameters, of various data types.
    

### Conditional statements

**If/Else statements**: Very often when you write code, you want to perform different actions for different decisions. You can use conditional statements in your code to do this. In Javascript, we have the following conditional statements:

* Use `if` to specify a block of code to be executed, if a specified condition is true
    
* Use `else` to specify a block of code to be executed, if the same condition is false
    
* Use `else if` to specify a new condition to test, if the first condition is false.
    
    ```javascript
    var hour = 24
    if (hour < 18) {
      greeting = "Good day";}
    else if (hour = 12) {
      greeting = "It is noon!" }
    else {
      greeting = "Good evening";
    }
    console.log(greeting)
    ```
    
    In the example above, we are telling the computer to give an output such that (`if`) the value of `hour` is &lt;18, it should log on the console "Good day". However (`else if`), if the value of `hour` =12, it should log on the console, "It is noon!". Then (`else`), if the value of `hour` is &gt;18, it should log on the console "Good evening".
    

**Switch statements**: Switch statements are an upgrade to the if/else statement. The `switch` statement specifies many alternative blocks of code to be executed.

* ```javascript
      var testScore = prompt("What is your score?");
      function grade(testScore) {
          switch (true) {
              case testScore <= 39: 
                  alert("You got an F!");
                  break;
              case testScore <=44:
                  alert("You got a E!");
                  break;
              case testScore <= 49:
                  alert("You got a D!");
                  break;
              case testScore <= 59:
                  alert("You got a C!");
                  break;
              case testScore <= 69:
                  alert("You got a B!");
                  break;
              case testScore <= 100:
                  alert("You got an A!");
                  break;
              default:
                  alert("You did not take the test!");
                 break;
          }
      }
      grade(testScore);
    ```
    
    Above, we have a function that takes a `switch` statement. We initially created a variable to store a user's input. We take the value of that input and analyze it with our `switch` statement such that if it is less than or equal to (`<=`) the number specified in either of our cases, the command inside the `case` block will be run. Think of each case as an `else if` statement.
    

### Loops in Javascript

Loops can execute a block of code as long as a specified condition is true.

* **While loops**: The `while` loop loops through a block of code as long as a specified condition is true.
    
    ```javascript
    while (i < 10) {
      text += "The number is " + i;
      i++;
    }
    ```
    
    In the above example, the code in the loop will run, over and over again, as long as a variable (i) is less than 10.
    
* **While..Do loop**: The `do...while` statements combo defines a code block to be executed once, and repeated as long as a condition is `true`. The `do...while` is used when you want to run a code block **at least one time**.
    
    ***If you use a variable in the condition, you must initialize it before the loop, and increment it within the loop. Otherwise, the loop will never end. This will crash your browser. If the condition is always true, the loop will never end. This will also crash your browser.***
    
    ```javascript
    let text = "Hello";
    let i = 0;
    do {
      text + "John";
      i++;
    }
    while (i < 5);
    ```
    
    Execute a code block `text + "John"` once, and then continue if condition (i &lt; 5) is true.
    
* **For loops**: The `for` statement defines a code block that is executed as long as a condition is `true`.
    
    `for (statement 1; statement 2; statement 3) {   code block to be executed }`
    
    * Statement 1: command to be executed before the code block starts. (Optional). This parameter can be omitted, but not the semicolon ";"
        
    * Statement 2: The condition for running the code block.  
        If it returns `true` the loop will start over again; otherwise, the loop will end. This parameter can be omitted, but not the semicolon ";"
        
    * Statement 3: command to be executed after the code block. This parameter can be omitted, but not the semicolon ";"
        
    
    ***If you omit statement 2, you must provide a break inside the loop.***
    
    ***Otherwise, the loop will never end. This will crash your browser.***
    

This was a long and interesting read!! We have been introduced to a lot of new concepts and ideas. I don't expect that you will understand this all at once, but going over the class twice or more, and following up with other classes will definitely put you on the right track.

That's all for today's (long) class. 🥳🥳 I'll see you all next week as we continue with our advanced Javascript class.

## References

* What is javascript
    
* [Keywords in programming](https://www.baeldung.com/cs/keyword-vs-reserved-word#:~:text=In%20computer%20programming%2C%20keywords%20are,that%20the%20program%20should%20perform.)
    
* [Javascript scope](https://www.w3schools.com/js/js_scope.asp)
    
* [Data types in javascript](https://devmountain.com/blog/what-are-data-types-javascript-101/#:~:text=In%20Javascript%2C%20there%20are%20five,booleans%2C%20undefined%2C%20and%20null.)
    
* [Image: variables in javascript](https://simplesnippets.tech/javascript-variables-data-types/)
    
* [Cover photo](https://www.google.com/url?sa=i&url=https%3A%2F%2Fgithub.com%2FTheAlgorithms%2FJavaScript&psig=AOvVaw1LphLLUo8_3tImoezdclH-&ust=1686926145769000&source=images&cd=vfe&ved=0CBMQjhxqFwoTCICIvOrkxf8CFQAAAAAdAAAAABAE)
    
* [Image: uses of javascript](https://www.educba.com/uses-of-javascript/)
    
* [Image: javascript functions](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.programiz.com%2Fjavascript%2Ffunction&psig=AOvVaw0LZhaqB2sxGGNX4W0Qg5CW&ust=1686934259088000&source=images&cd=vfe&ved=0CBMQjhxqFwoTCNio8_3dxf8CFQAAAAAdAAAAABAE)
    
* [Javascript functions](https://www.freecodecamp.org/news/what-are-functions-in-javascript-a-beginners-guide/#:~:text=A%20function%20is%20a%20block,prompt()%2C%20and%20confirm().)
    
* [Javascript if..else statements](https://www.w3schools.com/js/js_if_else.asp)
    
* [Javascript while loop](https://www.w3schools.com/js/js_loop_while.asp)
    
* [Javascript do..while loop](https://www.w3schools.com/jsref/jsref_dowhile.asp)
    
* [Javascript for loop](https://www.w3schools.com/jsref/jsref_for.asp)