---
title: "Javascript 99 bottles of beer solution"
seoTitle: "An easy solution to javascript 99 bottles algorithm challenge"
seoDescription: "Solve the 99 bottles on the wall algorithm with javascript using the floor loop in two easy steps."
datePublished: Mon Oct 24 2022 15:30:42 GMT+0000 (Coordinated Universal Time)
cuid: cl9mxr9nf00isaynv8aspe0qw
slug: javascript-99-bottles-of-beer-solution
cover: https://cdn.hashnode.com/res/hashnode/image/unsplash/08tX2fsuSLg/upload/v1666564886622/xOOhj-9lr.jpeg
tags: algorithms, javascript, easy, loops, solution

---

Hello and welcome! 🤩🤩🤩

I am super pumped writing this...

I am excited about many reasons, but the major one is that I have finally been able to crack this algo!!! 💃🏾💃🏾💃🏾

If you check on the internet, most solutions to this algorithm involve people using the `while` loop. Little secret, *I hate* `while` loops 😭😭

When I first learned the solution to this algorithm, it was with the `while` loop.

While preparing to write this article, I tried many times to replicate what I had learned, and what I had read on different javascript blogs.

After two laptop crashes, and a day of being completely frustrated, it occurred to me to give the solution a go with the `for` loop.

Trust me, the logic didn't come easy, but it came eventually, and I cleaned up my code, made it short, and made it very easy to understand.

Let's get to it!! 😁😁

As always, let us understand what is required of us in this algorithm challenge. *This is quite simple and straight to the point. There is a song with lyrics that you can find* [*here*](https://www.99-bottles-of-beer.net/lyrics.html)*. Your job is to replicate this song with your code, without hardcoding, and repeating multiple lines of code.*

### Step 1

The first step here is to define our loop.

```javascript
for (let numberOfBottles=99; 
numberOfBottles>=0; 
numberOfBottles--) 
{##insert code here}
```

*In our loop, we have defined the range we want our code to work in. That is, we want it to start from when the number of bottles is 99, down to when it is 0. We also want that, as our code runs/executes, it should be decreasing our* `numberOfBottles` by 1.

### Step 2

We will be using four conditional statements for the last parts of this solution. These conditional statements are because, at different points in our iteration, we want our lyrics to change and to accommodate grammatical changes also.

### 1st conditional:

```javascript
if (numberOfBottles > 2) 
{ console.log(numberOfBottles + " bottles of beer on the wall, " 
+ numberOfBottles + " bottles of beer.") 
console.log("Take one down and pass it around, " 
+ (numberOfBottles - 1) 
+ " bottles of beer on the wall.") }
```

*This is our very first conditional. You are probably wondering why it had to be* `numberOfBottles >2`, this is so because we will be needing to break our code when our iteration gets to 2 to accommodate for a grammar change.

### 2nd conditional:

`else if (numberOfBottles===2) { console.log(numberOfBottles + " bottles of beer on the wall, " + numberOfBottles + " bottles of beer.") console.log("Take one down and pass it around, " + (numberOfBottles - 1) + " bottle of beer on the wall.")`

*This 2nd conditional is to accommodate the grammar change for when it gets to* `1 bottle of beer...`

### 3rd conditional:

`if (numberOfBottles===1) { console.log("1 bottle of beer on the wall, 1 bottle of beer.") console.log("Take one down and pass it around, no more bottles of beer on the wall.")}`

\*In this 3rd conditional statement, we are telling our computer that when it keeps iterating and gets to the point where our `numberOfBottles` is equal to 1, it should modify our lyrics to suit the lyrics of the song. \*

### 4th conditional:

`else if (numberOfBottles===0) { console.log("No more bottles of beer on the wall, no more bottles of beer.") console.log("Go to the store and buy some more, 99 bottles of beer on the wall.") }`

*This is our fourth and final conditional statement. This is here to accommodate the lyrics change when there are no bottles of beer left on the wall. You will notice however that we have a hardcoded number there, on our last* `console.log`. This was a personal choice, as I did not see the need to go through the hoops of creating a separate variable for it. You can decide to do this on your own.

The full algorithm solution looks like this

```javascript
for (let numberOfBottles=99; numberOfBottles>=0; numberOfBottles--) {
   
   if (numberOfBottles > 2) {
       console.log(numberOfBottles + " bottles of beer on the wall, " + numberOfBottles +  " bottles of beer.")
      console.log("Take one down and pass it around, " +  (numberOfBottles - 1) + " bottles of beer on the wall.")
   }
   else if (numberOfBottles===2) {
       console.log(numberOfBottles + " bottles of beer on the wall, " + numberOfBottles +  " bottles of beer.")
      console.log("Take one down and pass it around, " +  (numberOfBottles - 1) + " bottle of beer on the wall.")
   }  
   else if (numberOfBottles===1) {
      console.log("1 bottle of beer on the wall, 1 bottle of beer.")
   console.log("Take one down and pass it around, no more bottles of beer on the wall.")
   }      
   else if (numberOfBottles===0) {
       console.log("No more bottles of beer on the wall, no more bottles of beer.")
      console.log("Go to the store and buy some more, 99 bottles of beer on the wall.")
   }
}
```

Awesome! That is the end of today's algorithm solution! Thank you for dropping by. 😁😁 Follow me on [Twitter](https://twitter.com/DumebiTheWriter) and on [Linkedin](https://www.linkedin.com/in/dumebi-okolo/)