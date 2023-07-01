---
title: "Build a vowel finder app with Javascript"
seoTitle: "Javascript project in four easy steps"
seoDescription: "Build this easy-to-build project with us in four easy steps. 
Step up your portfolio with this project."
datePublished: Mon Oct 17 2022 15:30:42 GMT+0000 (Coordinated Universal Time)
cuid: cl9cxob4400ayqgnvgpny8k1b
slug: build-a-vowel-finder-app-with-javascript
cover: https://cdn.hashnode.com/res/hashnode/image/unsplash/H7SCRwU1aiM/upload/v1667340905597/yIbIPSZ5N.jpeg
tags: css, javascript, web-development, projects, html5

---

Hello and welcome! 🤩🤩🤩

I got another project idea for you guysssss!!! 💃🏾💃🏾💃🏾💃🏾

I cannot overemphasize the need for these javascript projects we do here. These projects are easy to build, but they also cut across several fundamental aspects of javascript, so it feels like you are getting a load of practice for your javascript.

Let's get right to it!! 😁😁

Today, we'd be building a vowel finder app. Think of this as a word counter, only, it is a vowel counter! 🤣🤣

*The main idea of this app is that when you input a word or sentence, it returns the number of vowels present in your input.*

I should say that when you check the actual [website](https://dumebii.github.io/VowelFinder/) I built for this, you are going to choke on laughter. I made such a terrible mess of the CSS. 🤣🤣 I was just interested in creating the functionality. Fancy UI/UX was definitely not in the plan. That out of the way, let us get into the steps. [HTML](https://github.com/Dumebii/VowelFinder/blob/main/index.html) and [CSS](https://github.com/Dumebii/VowelFinder/blob/main/vowel.css) can be found here.

### Step 1

We are to create a function to call on our button. If you go through the HTML, you will see a button, which tells us the number of vowels we have when clicked.

```plaintext
      function vowelFinder() {
        var outputResult = document.querySelector("h3");
        var input = document.querySelector("#vowel-collector").value;
        console.log(input); }
```

*We fleshed out our function to collect two values*

\*&gt;&gt; We need a place to display our vowel count result. We are capturing this in an `h3` element in our HTML. We need a way to tap into and modify the text in our `h3`. this brought about the `outputResult` variable \*

*\&gt;&gt; We also need to capture our user's input, be it a word or sentence, or group of sentences. We do this with the* `input` variable.

### Step 2

We are adding some more variables to our function.

`var vowelCount=0;`

`var spreadInput= [...input];`

*Our first variable* `vowelCount` is what we are going to use to keep track of the number of vowels we get. It will auto-update once there is a new vowel detected.

\*Then we have the `spreadInput` variable. This is a big one because it has us using the ES6 `spread` operator. Basically, what this basically does, is that it takes the input we get from our user, and "spreads it out" such that we are able to scan each letter individually to find out if it is a vowel or not. \*

### Step 3

Here comes the logic part of our app. We will be using a `for` loop, and the `switch` statement. I will write out the code, and explain under.

```plaintext
    for (let val of spreadInput) {
    switch(val) {
        case "a":
        vowelCount++
        break;
        case "e":
        vowelCount++
        break;
        case "i":
        vowelCount++
        break;
        case "o":
        vowelCount++
        break;
        case "u":
        vowelCount++
        break;
    }}
```

\*The essence of having a `for` loop is that we will be required to loop through each letter of our output, through the `spreadInput` variable, which is already storing this. \* *Side note: if you notice in our* `for` loop, we only have one condition in our parenthesis, unlike the usual two or three. This is because we do not need an endpoint in our loop. We want it to continue parsing until every `val` in our `spreadInput` variable has been checked.

*We are using the* `switch` statement in this case because we have a lot of conditions to be met. In each of our cases, we are checking to see if the presence of the stated vowel is true. If it is true, we need our computer to update our `vowelCount`.

### Step 4

Yaaaayyy!!! Our final step! We are done with all the heavy lifting! This step is basically for us to output the result of our `vowelCount` when we are done parsing through our input.

`outputResult.innerHTML = "The total number of vowels is " + vowelCount;`

Our total function will look like this

```plaintext
  function vowelFinder() {
    var outputResult = document.querySelector("h3");
    var input = document.querySelector("#vowel-collector").value;
    console.log(input);
    var vowelCount=0;
    var spreadInput= [...input];
    for (let val of spreadInput) {
      switch(val) {
        case "a":
        vowelCount++
        break;
        case "e":
        vowelCount++
        break;
        case "i":
        vowelCount++
        break;
        case "o":
        vowelCount++
        break;
        case "u":
        vowelCount++
        break;
    }}
    outputResult.innerHTML = "The total number of vowels is " + vowelCount
}
```

*Our function is being called in our HTML, with the* `onclick` attribute in our button tag.

That's all for today, folks! Thank you for stopping by. Follow me on socials [twitter](https://twitter.com/TheTechSis) [Linkedin](https://www.linkedin.com/in/dumebi-okolo/)