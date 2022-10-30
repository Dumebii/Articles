# Javascript fizzBuzz solution

Hello and welcome!! 🤩🤩

I think that honestly, one of the rights of passage anyone has to pass through when learning any programming language is to figure out the `fizzBuzz` challenge!
It is one of the first algorithm solutions that you are taught. 
In the case of javascript, it is actually a brilliant way to get you started and knowledgeable about some key aspects of the javascript language. 

**Let's get right to it!**

As always, I will like to begin my solutions with first of all understanding what the problem is. 

*The fizzBuzz challenge is such that you are mostly to return a set of numbers from 1-100 such that any number divisible by 3 has an output of "fizz", whereas any number divisible by 5 has an output of "buzz."
However, any number divisible by both 3 and 5 should have an output of "fizzBuzz." *

From looking at this, we can immediately see that there are two core principles we need:

1. Conditional statements.
2. A means to iterate/loop over our set of numbers. 

We will be using the `if-else` statement for the conditional statement and the `for` loop for the iteration. 

### Step 1
Create a function that can be called to carry out the process.  

` function fizzBuzz() {}`

### Step 2
We need to implement our `for` loop. 

`for (let i = 0; i < 100;  i++)`

*This expression above simply means that we are staring out counting from i = 0, ending at i < 100, and incrementing `i` per iteration*

### Step 3
We have three conditons that need to be met. 
i. When it is divisible by 3
ii. When it is divisible by 5
iii. When it is divisible by 3 and 5.

*We will be starting with the "last" condition, that is, when i is divisible by both 3 and 5, and this is because javascript reads from top to bottom, and we do not want it to parse through all the numbers first finding conditions i & ii, because by the time it does all this, even the numbers divisible by both 3 and 5 would be taken up by "fizz"  seeing as it is the first condition to be encountered. *

i. **When it is divisible by both 3 and 5.** 

Now, there are two statements that you can use to write this:

`if (i % 3 === 0 && i % 5 === 0) {
console.log("fizzBuzz")};`

or 

`if (i % 15 === 0) {
console.log("fizzBuzz")}`

*Both statements basically do the same thing, just that the second statement used 15 as the **Lowest Common Multiple** of both 3 and 5. *

ii. **When it is divisible by 3:**

` else if (i % 3 === 0) {
console.log("fizz")}; `

*The modulo sign `%` is used here because we need each value of i to be entirely divisible by 3, which means that `i % 3` has to be = 0. *


iii. **When it is divisible by 5:**

` else if (i % 5 === 0) {
console.log("buzz")}; `

*The modulo sign `%` is used here because we need each value of `i` to be entirely divisible by 5, which means that `i % 5` has to be = 0. *


### Step 4
Our `else` statement:

`else { console.log(i)};`

*This is to ensure that all other numbers that did not satisfy any of the 3 conditions above get captured. *

The final code would look like this:

```
function fizzBuzz() {
 for (i = 1; i < 100; i++) {
  if (i % 15 === 0) {
   console.log("fizzBuzz")};
  else if ( i % 3 === 0) {
    console.log("fizz")};
  else if ( i % 5 === 0) {
    console.log("buzz")};
  else {
     console.log(i)};
```

And that's it, folks! 
I hope you have as much fun coding this out as I did writing it! 
Until next time. ❤❤








