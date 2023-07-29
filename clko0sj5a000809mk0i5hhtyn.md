---
title: "Javascript Array Methods"
seoTitle: "Javascript array methods to learn"
seoDescription: "What is the JavaScript map method? How to use the Javascript filter method, forEach method for web development"
datePublished: Sat Jul 29 2023 13:00:12 GMT+0000 (Coordinated Universal Time)
cuid: clko0sj5a000809mk0i5hhtyn
slug: javascript-array-methods
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1690582817521/9672d4f1-c843-4006-9309-6bb32f5f94c4.jpeg
tags: tutorial, javascript, web-development, beginners, array-methods

---

Hello and welcome!! 🤩🤩🤩

In this article, we will be looking at four of the modern Javascript Es6 array methods: `map()`, `forEach()`, `filter()`, `reduce()` methods.

## What are methods in Javascript?

JavaScript methods are incredibly useful for performing various actions on objects. Essentially, a JavaScript method is a property that holds a function definition, which makes it easy to work with objects programmatically. Whether you're manipulating the DOM, handling user input, or performing complex calculations, JavaScript methods provide a powerful and flexible toolset for developers to work with. So if you're looking to take your web development skills to the next level, mastering JavaScript methods is a smart move!

## The Javascript map() method

The `.map` method allows you to iterate through an array and carry out a specific function call for each of the array items. This will create a new array in which the changed array items are contained.

The general syntax for the map method is:

`array.map(function to be carried out on each item)`

```javascript
//map method with a function call 
const numbers = [1, 2, 3, 4, 5];
function double(x) {
  return x*2;
};
const newNumbersArray = numbers.map(double);
console.log(newNumbersArray);

//console output = [2, 4, 6, 8, 10]

//map method with an annonymous function call 
const anotherNumbersArray = numbers.map((x) => {return x*3});
console.log(anotherNumbersArray);
//console output = [2, 4, 6, 8, 10]
```

In the codepen above, there are two examples of how the `map` method works.

In the first example, we defined a function outside the map method. The function we defined takes in the command we want to happen to each of the items in the array. The second example sees us using an `arrow function` to define our function call directly inside the method.

## Javascript forEach() method

The `forEach` method calls a function for each element in an array.

The `forEach` method is similar to the `map` method in that it iterates over the items in an array with a function.

However, the difference between a `forEach` method and a `map` method is that a `map` method returns a new array of the modified array items while a `forEach` method returns undefined.

We use a `forEach` method when we have a small array to iterate over, as it is faster than the `map` method.

```javascript
const numbers = [1, 2, 3, 4, 5, 6, 7];
const newArray = [];
 numbers.forEach((x) => {newArray.push(x*2)})
console.log(newArray);
//console output = [2, 4, 6, 8, 10, 12, 14]
```

You will notice in the example above that we had to create a new array ourselves and add our updated list items to it.

## Javascript filter() method

What the filter method does is that it returns, in a new array, the array items that satisfy/meet the condition embedded in the function.

```javascript
const numbers = [10, 2, 13, 4, 50, 60, 7];
const newArray = numbers.filter((x) => {return x > 10});
console.log(newArray);

// console output = [13, 50, 60]
```

We see that in the new array `newArray` that the numbers returned are the ones that satisfy the condition in the function. That is, it returned numbers that were greater than 10.

## Javascript reduce() method

The `reduce()` method executes a reducer function for an array element. The `reduce()` method returns a single value: the function's accumulated result. The `reduce()` method does not execute the function for empty array elements. The `reduce()` method does not change the original array.

```javascript
const numbers = [10, 2, 13, 4, 50, 60, 7];
numbers.reduce((total, num) => {return total * num})
// output = 21840000
```

The `reduce` method takes two required parameters, total and currentValue.

The reduce method does a scalar operation on the array, which is a vector. In a scalar operation (addition, multiplication, subtraction, or division) of a vector (array), only one value is returned.

Think of the total parameter as the present value or the current array. The current value is the individual values in the array.

We can now determine the scalar operation we want to happen on the array or vector. In the case of the example above, each item on the array, starting from `index 0` is multiplied by each other to make one single unit value.

That's the end of this article for today! Thanks for dropping by. I hope you had as much fun reading this as I did writing it.

Follow me [Linkedin](http://www.linkedin.com/in/dumebi-okolo)