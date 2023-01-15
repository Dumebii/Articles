# React Hooks Explained

Hello and welcome!!

Today, I'd be sharing my knowledge on three of my favorite React hooks that I have learned. I will try my best to explain this as simply as I can, the way that I understand it. Hopefully, this can help fuel your understanding.

***Please note that this article is not holistic nor does it aim at teaching you everything that you need to know.***

# HOOK 1

# useState

This is one of the foremost things you will learn in React. React's `useState` is used to add functionality to your react app. A simple way of understanding what the `useState` is all about thinking of the current condition of your website as in a 'state'. What useState then helps you to do is update the particular state of your website.

The general syntax of the `useState` uses the array destructuring principle. We have two parameters in the destructured array: the value for which the current state of your website is represented, and the second which is to help us to set the state we want to be updated.

```javascript
import { useState } from 'react'

function App() {
const [state, setState] = useState("Obi is a boy!");
  return (
    <h1 onClick={ () => setState("Obi is now a girl!") }> {state} </h1>
  )
```

*In the simple code snippet above, we see our initial state being a* `h1` *saying that "Obi is a boy!" However, we want that when we click on the h1, it changes the value to show "Obi is now a girl!"*

*We see how by the use of useState, we are able to add functionality to our websites. We can store all sorts of values in our initial state, from booleans to arrays, to objects.*

**The** `useState` **hook is a lot deeper than this and gets more complicated the further down you go. This is just an overview to give a general understanding of it.**

# HOOK 2

## useEffect

The most important feature (in my opinion) to note about React's `useEffect` hook is that in it you put something that you want to run/be rendered after a certain action has been completed.

* A typical `useEffect` syntax takes two inputs: the first input which is the action/function you want to be run/performed, and then a second arguement called a `dependencies array`. This dependency array is probably the most important part of the syntax. This ensures your initial input isn't carried out until what is in the dependency array is carried out/run/executed.
    

```javascript
import { useState, useEffect } from 'react'

function App () {

 const [boolean, setBoolean] = useState(false);
        
       useEffect(() => {
       console.log("This should execute")}, [!boolean])
        
return (
        
       <h1 onClick={()=> setBoolean(!boolean) }> Hello World! </h1>
        
       )}
```

*This means that the* `console.log` given as the first argument in the `useEffect` syntax would not run unless only the condition "not boolean" is satisfied. Boolean is a state variable whose updating is dependent on the `onClick` event in the `h1` being triggered. What this simply means is that the `console.log` would not take effect till the `h1` is clicked.

*Note though that sometimes, the* `dependencies array` *is empty. What this means is that we want the* `console.log`, *as in the example above, to run only once, and immediately the page is rendered.*

* The `useEffect` hook can, and should be used for other "more important" things in a React app though. Primarily managing fallout or effects from using *external bodies* on a React app, like making an API call, amongst other things that React typically isn't built to handle.
    

**The** `useEffect` **hook is a lot deeper than this and gets more complicated the further down you go. This is just an overview to give a general understanding of it.**

# HOOK 3

## useRef

I'd like to think of this as my favorite react hook. This is because it allows me to do the one thing I had previously found challenging in React. Think of the `useRef` hook as react's equivalent to vanilla javascript's `document.querySelector` to target an element.

```javascript
import { useRef } from 'react'

function App() {
 const exampleRef = useRef()
 return ( 
   <h1 ref={exampleRef} onClick={ () => exampleRef.current.textContent = "It is evening now!" }> Hello! Morning! </h1>
) }
```

*What the above code snippet helps us see is that we can access the* `textContent` *of our* `h1` *tag, and change it to something else, just as we would have easily done with a* `document.querySelector`*. This of course happens when we trigger the* `onClick` *event on the h1.*

In some instances, as we did above, we can afford to use the `useRef` hook in place of a `useState` hook when we want to make sure that the website does not re-render unnecessarily. That is, we could have easily achieved our goal using the `useState` hook, but in instances like this where we do not require re-renders, it is better to use the `useRef` hook.

**The useRef hook does not cause site re-render.**

**The** `useRef` **hook is a lot deeper than this and gets more complicated the further down you go. This is just an overview to give a general understanding of it.**

I will suggest [this blog](https://www.smashingmagazine.com/2020/11/react-useref-hook/) to have a better understanding of the react `useRef` hook, and its relationship with the `useState` hook.

Thank you for stopping by, and I hope you had as much fun reading this article as I did writing it!

Untill next time. ❤❤❤