---
title: "Advanced Javascript... All you need to know, and more"
seoTitle: "Advanced Javascript principles. Array destructuring. Spread operator."
seoDescription: "What are arrays and objects in javascript and how to use them? Javascript functions, types, uses and examples. Javascript array and object destructuring."
datePublished: Thu Jun 22 2023 14:57:09 GMT+0000 (Coordinated Universal Time)
cuid: clj79ofbo000q09k2adog7rol
slug: advanced-javascript-all-you-need-to-know-and-more
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1687392010300/9e4bb308-5ed2-4233-b648-66394ca8dd3a.png
tags: tutorial, javascript, web-development, frontend-development, advance-javascript

---

Hello and welcome!! 🤩🤩🤩

In this week's class, we will continue on our Javascript journey, learning about more advanced Javascript topics and getting our hands dirty with examples.

## What is '**this'**?

In JavaScript, the `this` keyword refers to an **object**.

**Which** object depends on how `this` is being invoked (used or called).

The `this` keyword refers to different objects depending on how it is used:

<table><tbody><tr><td colspan="1" rowspan="1"><p>In an object method, <code>this</code> refers to the <strong>object</strong>.</p></td></tr><tr><td colspan="1" rowspan="1"><p>Alone, <code>this</code> refers to the <strong>global object</strong>.</p></td></tr><tr><td colspan="1" rowspan="1"><p>In a function, <code>this</code> refers to the <strong>global object</strong>.</p></td></tr><tr><td colspan="1" rowspan="1"><p>In a function, in strict mode, <code>this</code> is <code>undefined</code>.</p></td></tr><tr><td colspan="1" rowspan="1"><p>In an event, <code>this</code> refers to the <strong>element</strong> that received the event.</p></td></tr></tbody></table>

## Data types cont'd

### Arrays in Javascript

In JavaScript, an array is **an ordered list of values**. Each value in an array is called an element and is identified by an index. An array can hold values of mixed types. For example, you can have an array that stores elements with the types number, string, boolean, and null.

```javascript
var anArray = ["hello", 1, null, false];
```

The above is the more common way of writing out an array in Javascript.

However, there is another way: using the `Array` constructor function.

```javascript
var emptyArray = new Array();
var controlledArray = new Array(6);
var anArray = new Array(1, 'hello', null, false];
```

The example above has three examples using the `Array constructor function`. In the first line, what we have done is initialize an empty array. That is, we have opened up a 'box' or 'container' in which to store our data. This creates flexibility in that it allows our array to take any number of data inputs. In the second line, we have a controlled array. A controlled array in that we have specified a total number of values that the array is allowed to store or carry. In this case, we have made it so that `controlledArray` can only have six values. In the last line, we have initialized an array, as we did in the first code example above.

A way to initialize an empty array or the syntax for an array in javascript is

`var emptyArray = []`

As earlier stated, values in a Javascript array are identified by their index. In programming, we start our indexing from 0, not 1.

`var array = [1,2,3,4,5];`

**Accessing values**

From `array` above, our value '1' is indexed at 0. Subsequently, '2' is indexed at 1, and so on. This is a concept new programmers often struggle with (I know I did 😅), but in time and with frequent practice, it becomes second nature knowledge to you.

***Note: When we start indexing from reverse, that is, from the end of a value to the beginning, we start our index from -1. That is, from the example above, in reverse counting, the index of '5' is -1.***

To pick off a value in an array by its index, we use the following syntax:

```javascript
var array = [1, 2, 3, 4, 5, 6];
console.log(array[1], array[4], array[0]);

//console output: 2, 5, 1
```

### Objects in Javascript

An object in JavaScript is an unordered collection of key-value pairs. Each key-value pair is referred to as a property. A property's key can be a string. A property's value can be anything, such as a string, a number, an array, or even a function. There are numerous ways to construct an object with JavaScript. The object literal notation is the most often used.

```javascript
var objectExample = 
{name: 'John',
 num: 15754, 
isEducated: false,
runOnce() {return 'I ran once!'}
};
```

**Accessing properties:**

To access a property of an object, you use one of two notations: the `dot notation` and `array notation`.

```javascript
var objectExample = 
{name: 'John',
 num: 15754, 
isEducated: false,
runOnce() {return 'I ran once!'}
};
console.log(objectExample.num) //this is the dot notation
console.log(objectExample['isEducated']); //this is the array notation

/*
console output: 
objectExample.num: 15754
objectExample['isEducated']: false
*/
```

## Methods in Javascript

An object is a collection of key/value pairs or properties.

There are a lot of JavaScript methods that are useful to our progress in JavaScript development. I will only touch on two in this article. However, you can read about more Javascript methods and how you can use them [here](https://www.tutorialspoint.com/javascript/javascript_builtin_functions.htm).

### String methods

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1687395881483/c030f5f8-4191-46fe-9b6d-95926c0c8fd0.png align="center")

String methods are methods that we can use on strings to either modify them or read their values.

**String length:** This is a string property that tells us the number of characters contained in a string.

```javascript
var string = 'string';
var length = string.length;
console.log(length);

//console output: 6
```

Properties or methods are attached after a `dot notation` at the end of our variable name. In the above code block, we see that the `length` property was attached with a `dot notation` at the end of our variable name `string`.

**String extraction**

There are 3 methods for extracting a part of a string:

* `slice(start, end)` : this specifies to extract a string from the start of an index to the end of the index.
    
* `substring(start, end)` : in this method, any negative index is treated as starting from index zero.
    
* `substr(start, length)` : in this method, the second parameter is used to specify the length(or extent) to which we want the string extracted.
    

```javascript
var text = 'This is a full text.';
var slice = text.slice(5, 11);
var substring = text.substring(-5, 11);
var substr = text.substr(5, 11);
console.log(slice, substring, substr);

/* console output: 
slice: is a f 
substring: This is a f 
substr: is a full t
*/
```

In the code block above, we see that with `.slice`, we got the string sliced from index 5 to index 11. But we see something funny here. The extraction does stop at 10. Yes, that is because in programming, when selecting a range, we start from the beginning of the range to the number just before the end of the range. So, as in the example above, our extraction stopped at index 10.

***Please note that in a string such as the one we have above, whitespaces are indexed as well.***

**Converting to upper and lower cases**

A string is converted to uppercase with `toUpperCase()`

A string is converted to lowercase with `toLowerCase()`

```javascript
var example1 = 'hello';
var upperCase = example1.toUpperCase();
var example2 = 'HELLO';
var lowerCase = example2.toLowerCase();
console.log(upperCase, lowerCase);

/*
console output: 
upperCase: HELLO
lowerCase: hello
*/
```

For more string methods, and the beautiful things we can do with them, check out W3School's [documentation](https://www.w3schools.com/js/js_string_methods.asp) on string methods.

### Array Methods

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1687398887861/ac1a79e7-ef6f-47cc-aed9-873b6952014d.png align="center")

**Array Length**

The array length property serves the same purpose as the string length property in that it is used to tell the length of an array.

```javascript
var array = ['hello', 1, null, false];
console.log(array.length);

// console output: 4
```

**Popping and Pushing**

When you work with arrays, it is easy to remove elements and add new ones.

This is what popping and pushing are: Popping items **out** of an array, or pushing items **into** an array.

```javascript
var salutations = ['Hello', 'Hi', 'Hey', 'Howdy']
salutations.pop();
console.log(salutations);
salutations.push('Ekaroo');
console.log(salutations);

/*
console output: 
salutations.pop(): ['Hello', 'Hi', 'Hey']
salutations.push('ekaroo'): ['Hello', 'Hi', 'Hey', 'Ekaroo']
*/
```

For more on array methods, and the beautiful things we can do with them, check out W3School's [documentation](https://www.w3schools.com/js/js_array_methods.asp) on array methods. Also, check out this [amazing article](https://medium.com/@mandeepkaur1/a-list-of-javascript-array-methods-145d09dd19a0) on JavaScript array methods.

## Array and object destructuring in Javascript

The destructuring assignment is a cool feature that came along with ES6. Destructuring is a JavaScript expression that makes it possible to unpack values from arrays, or properties from objects, into distinct variables. That is, we can extract data from arrays and objects and assign them to variables.

```javascript
let array = [1, 2, 'kitty', 4, 5, 6, 7];
let [1, 2, 3, 4, 5, 6, 7] = array;
console.log(3);

//console output: kitty
```

This might seem as though we almost reversed our array. What we did was assign a *variable name* to each item/value in our array, to make it easy for retrieval. Instead of typing `array[3]` to get the item at index `3`, all we had to do was type in '3'. You can read more about destructuring [here](https://www.freecodecamp.org/news/array-and-object-destructuring-in-javascript/).

## Functions and types of functions

A JavaScript function is a block of code designed to perform a particular task.

A JavaScript function is executed when "something" invokes it (calls it).

Get a better introduction to functions in Javascript from our [lesson](https://dumebi.hashnode.dev/learn-front-end-web-development-in-12-days-beginner-javascript) last week.

Broadly speaking, JavaScript has four kinds of functions:

* **Regular function**: can return anything; always runs to completion after invocation
    
    The general syntax for a JavaScript function is
    
    ```javascript
    function thisIsAFunction() {
    //Enter function code block here
    }
    ```
    
* **Generator function**: returns a [`Generator`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Generator) object; can be paused and resumed with the [`yield`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/yield) operator
    
* **Async function**: returns a [`Promise`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise); can be paused and resumed with the [`await`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/await) operator
    
    ```javascript
     async function thisIsAFunction() {
    //Enter function code block here
    }
    ```
    
* **Async generator function**: returns an [`AsyncGenerator`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/AsyncGenerator) object; both the `await` and `yield` operators can be used
    

### Function return statement in JavaScript

When JavaScript reaches a `return` statement, the function will stop executing.

If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement.

Functions often compute a **return value**. The return value is "returned" back to the "caller".

```javascript
function myFunction(a, b) {
  return a * b;
// Function returns the product of a and b
}
console.log(myFunction(5, 6));

//console output: 30
```

### Arrow functions

An [arrow function expression](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions) (also called a *fat arrow* to distinguish it from a hypothetical `->` syntax in future JavaScript) has a shorter syntax compared to function expressions and does not have its own [`this`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this). Arrow functions are always anonymous.

Two factors influenced the introduction of arrow functions: *shorter functions* and the *non-binding* of `this`.

```javascript
const arrow = () => {return 'Her name is Chloe'}
arrow()
```

The above is a standard syntax for an arrow function. Arrow functions are very effective for writing in-line functions or for returning only one value.

```javascript
function fizzBuzz() {
    for (let i = 0; i < 100; i++) {
        if (i % 15 === 0) {
            console.log("fizzBuzz")
        }
        else if (i % 3 === 0) {
           console.log("fizz") 
        }
        else if (i % 5 === 0) {
            console.log("Buzz")
        }
        else {
            console.log(i) 
        }
    }
}

fizzBuzz()
```

The above code block is an example of a function solving the famous Fizzbuzz algorithm challenge. I detail more about this solution [here](https://dumebi.hashnode.dev/javascript-fizzbuzz-solution).

## Javascript Spread operator

This is my favorite thing about ES6! 🤣

The JavaScript spread operator (`...`) allows us to quickly copy all or part of an existing array or object into another array or object.

```javascript
var firstSixNumbers = [1, 2, 3, 4, 5, 6];
var firstTenNumbers = [...firstSixNumbers, 7, 8, 9, 10];
console.log(firstTenNumbers);

//console output: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
```

We see above how we did not have to copy all the values from our first array into the second one. We simply had to *spread* it in the second one. Imagine how useful this will be for an array with a longer length or more!

Hi, guys! That's all for this week and our lesson on vanilla javascript. From next week, we will be looking at javascript for web development starting with learning about the DOM manipulations. See you all next week!!

## References

* [Cover Image](https://www.google.com/url?sa=i&url=https%3A%2F%2Fcodeberryschool.com%2Fblog%2Fen%2Fjavascript-a-programming-language%2F&psig=AOvVaw2c3YkLyBA2hf6yO1Y1RtzJ&ust=1687478265461000&source=images&cd=vfe&ved=0CBMQjhxqFwoTCIi0jcvI1f8CFQAAAAAdAAAAABAE)
    
* [Javascript Arrays](https://www.javascripttutorial.net/javascript-array/#:~:text=In%20JavaScript%2C%20an%20array%20is,string%2C%20boolean%2C%20and%20null.)
    
* [Javascript objects](https://www.javascripttutorial.net/javascript-objects/)
    
* [String methods](https://www.w3schools.com/js/js_string_methods.asp)
    
* [Array methods](https://www.w3schools.com/js/js_array_methods.asp)
    
* [Methods in Javascript](https://www.javascripttutorial.net/javascript-object-methods/)
    
* [Functions in javascript](https://www.w3schools.com/js/js_functions.asp)
    
* [Arrow functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions)
    
* [Types of functions in Javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions)
    
* [What is 'this'?](https://www.w3schools.com/js/js_this.asp)