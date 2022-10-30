# Simple Javascript project ideas

Hello and welcome! 🤩🤩

When you journey into web development, there are tiers of challenges, and conquering javascript is one of them!
In my experience, learning javascript is best done through practice. it is possible to watch a ton of tutorial videos, you'd think you've got it nailed, only to end up with very faulty code. 

In this article, we will be building a straightforward javascript game. This challenge will have you practicing some beginner and core principles of javascript programming. As a bonus, you even get a bit of an HTML and CSS lesson. 

Let's kick right into what we'd be building!

**Today, we'd be building the popular British game called The Simon game**

I have learned through experience that the secret to solving coding challenges is to, first of all, understand what's required of you.
To achieve this, we will have to understand how the Simon game works.  Find a youtube tutorial video [here](https://www.youtube.com/watch?v=EWJ5uYwQJGU). 

Let me try my best to explain. 

This is primarily a pattern remembrance game. This game is in such a way that there are four boxes. Each box is a different color. The game starts with a "Press any key to play" heading. Once you've done this, a box(with a particular color) is highlighted, and the highlight fades after a millisecond. This represents the first pattern. You are to click on the box that was highlighted. *You have successfully remembered the first pattern.*

The game highlights another color...

But remember, it's all about patterns 😜😜 If you click on the following highlighted pattern, you fail! 😭😭😭 (I learned this the hard way). Because this is a game of patterns, you have to remember the first color(box) that was highlighted and start from there.

> Example:
> The patterns show up in this order [Blue] 1st highlight: play [blue 🔵]
> 
> [Red] 2nd highlight play [blue 🔵][red 🔴]
> 
> [Green] 3rd highlight play [blue 🔵][red 🔴][green 🟢]
> 
> [Blue] 4th highlight play [blue 🔵][red 🔴][green 🟢][blue 🔵]....
The game keeps going on in a continuous loop until you miss a pattern and then it restarts.

Get a feel of playing the game [here](https://dumebii.github.io/Simon-Game/) 

Because this is neither an HTML or CSS tutorial, I'd be dropping a link to the [HTML](https://github.com/Dumebii/Simon-Game/blob/main/index.html) and [CSS](https://github.com/Dumebii/Simon-Game/blob/main/styles.css) codes. You can grab those, get them running in your preferred code editor, open up a javascript file, and let's get started!

### Step 1
The first thing we have to think about is that we need to define the colors of the buttons. In my HTML file, you can see that we have four divs with ids of different colors (red, blue, green, and yellow), to identify each box separately. 
We can do this in our javascript by first of all creating an array 


`var buttonColors = ["red", "blue", "green", "yellow"];
` 


### Step 2
We need a way to store the patterns the game is going to come up with and also the pattern that our user is going to be creating (by playing the game), so that we can keep track of it. 

`var gamePattern = [];
      var userClickedPattern = [];
`

### Step 3
We need to create a function that enables the game to choose which of the buttons it wants to add in the sequence. 
We recall from the explanation of the game that this isn't a rigid structure, such that the computer spins off random patterns. 
To achieve this, let us create our function, and get a randomized variable. 

`function nextSequence() {
  var randomNumber = Math.floor(Math.random()*4);}
`

*We are multiplying our random number by 4 so that we can have values between o and 3. Using a 'Math.floor' method to remove any floating point from our number.*

### Step 4
We need to make use of our randomized variable to help us pick a random index from our 'buttonColors' array. We will also need to find a way to add the value of the chosen index (the first sequence in the game) to our game pattern array.

`
      var randomChosenColor = buttonColors[randomNumber];
       gamePattern.push(randomChosenColor);  
`

### Step 5

Now, we are going to add a bit of animation, as a visual cue to indicate what color (box) was chosen by the computer. 

`document.querySelector("#" + randomChosenColor).fadeIn(100).fadeOut(100).fadeIn(100);
`

*We used the `document.querySelector` to target the HTML element we want. What we need is identified with an id, hence why we had to use the id selector "#". Furthermore, because we are not hardcoding any particular value, but letting the computer choose randomly, we had to write our code so that the selection is fed from our 'chosenRandomColor' variable.*


Our `nextSequence` function should look like this,


```
function nextSequence() {
    userClickedPattern = [];
    var randomNumber = Math.floor(Math.random()*4);
    var randomChosenColor = buttonColors[randomNumber];
    gamePattern.push(randomChosenColor)
    document.querySelector("#" + randomChosenColor).fadeIn(100).fadeOut(100).fadeIn(100);
}
``` 

### Step 6 
In addition to the visual aid introduced in our earlier function, we can also add some sound cues. 
We will be doing this in our `playSound()` function. 
You can find the sound used for this project at [this github repo](https://github.com/Dumebii/Simon-Game/tree/main/sounds). 
We will be using the default audio class in javascript. 

```
function playSound(audioName) {
    var audio = new Audio("sounds/" + audioName + ".mp3");
    audio.play();
}
```

*Our function takes a parameter of `audioName` such that we use this parameter to pass in the value of the name of the audio we want to use. After getting hold of the default audio class in javascript, we went ahead to get a hold of the different sounds by giving it a 'filer' with our `audioName` parameter. We will see the implementation of this in coming functions. *

### Step 7 
We need to build a function that helps the track be aware of what button they clicked. This is by adding some sort of visual aid/clue as to which button was pressed by the user. 

```
function animatePress(currentColor) {
    document.querySelector("#" + currentColor).addClass("pressed");
    setTimeout(function () {
    document.querySelector("#" + currentColor).removeClass("pressed");
  }, 100);
}
```

*In our `styles.css` there is a class name 'pressed'. What we did here is use javascript to toggle off and on our class `pressed`. Toggling on this class simply increases and decreases opacity. Note also that we used the `setTimeout` function to set the duration for the toggle off and on. *

### Step 8

Our game is looking fine so far, but there is no way to actually track if the user is following the pattern set by the computer, and that is exactly what this next function is for. 
We write our first 'if' statement. 

```
if (gamePattern[currentLevel] === userClickedPattern[currentLevel]) {
      if (userClickedPattern.length === gamePattern.length){
        setTimeout(function () {
          nextSequence();
        }, 1000);
      }
    }

```

*In this `if` statement, the conditions we are checking for the concurrency of the index of our game's pattern with the index of our user's pattern. This will enable us to know when a user has overshot the sequence, or underused. It also checks that the length of each of the arrays is the same. If both cases prove to be true, our earlier function  `nextSequence` is triggered. *

We of course need to close this off with an else statement that checks for when the user doesn't get the sequence correctly. 

```
else {
      playSound("wrong");
      document.querySelector("body").addClass("game-over");
      setTimeout(function() {
          document.querySelector("body").removeClass("game-over");
      }, 200);
      document.querySelector("h1").text("Game over! Press Any Key To Restart");
     //startOver()
    }
```

*In this `else` statement, we are triggering another CSS class `game-over` and toggling it off and on. There is a commented-out function here. You will understand it later as it will be explained shortly.  *

Our final function should look like this:

```
function checkAnswer(currentLevel) {
    if (gamePattern[currentLevel] === userClickedPattern[currentLevel]) {
      if (userClickedPattern.length === gamePattern.length){
        setTimeout(function () {
          nextSequence();
        }, 1000);
      }
    } else {
      playSound("wrong");
      document.querySelector("body").addClass("game-over");
      setTimeout(function() {
          document.querySelector("body").removeClass("game-over");
      }, 200);
      document.querySelector("h1").text("Game over! Press Any Key To Restart");
      //startOver();
    }
}

```


### Step 9
We need a way for the user to play the game. That is, we have to add functionality to our buttons. We will be using the `.click` method. 
In the function that is to be included in this method, we need to specify a list of things that we want to happen by the functions we have so far 

```
   document.querySelector(".btn").click(function() {
    var userChosenColour = document.querySelector(this).attr("id");
    userClickedPattern.push(userChosenColour);
    playSound(userChosenColour);
    animatePress(userChosenColour);
    checkAnswer(userClickedPattern.length-1)
     });
```
*When we press this button, a bunch of things are going to happen. The first thing we are doing is to capture the id of the clicked button and store it in our `userChosenColor` of our clicked button. This is achieved using the 'this' keyword. Then we populate our `userClickedPattern` array, of course, with whatever color(button) the user chooses.  We bring in some of our already defined functions which take in our `userChosenColor` as arguments. *


### Step 10
Finally! We need a way to make sure that the user is able to restart the game whenever they miss a sequence. 
We will achieve this with our `startOver` function.
We first need to create a variable at the beginning of our file that keeps track of when the game has started or not, 

`var started = false;
`
Then our function becomes 

```

function startOver() {
  gamePattern = [];
  started = false;
}

```

*We can see here that in our function, we are merely restarting everything, and making sure that everything begins on a new slate. Please, go back to your `check answer` function, and uncomment our `startOver()`*


We are almost at the end of the road, guys!!! 🥳🥳🥳

The final thing we need is a way to keep track of when our game begins. 

```
document.querySelector(document).keypress(function() {
    if (!started) {
        document.querySelector("h1").text("Level " + level);
        nextSequence();
        started = true;
    }
});
```

Yasssss!!! 🥳🥳🥳
We are done with our first javascript project!
Writing this has been an exciting experience. I hope you feel the same excitement when you build this game and show it off to your friends. 

Thank you for stopping by! 



