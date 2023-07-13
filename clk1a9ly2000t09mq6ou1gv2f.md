---
title: "React for beginners: an overview"
seoTitle: "React for beginners. An overview of React for beginners"
seoDescription: "This article talks about the javascript frameworks. We learn about, React JSX, functional components, React Hooks, and how to build a counter app with React"
datePublished: Thu Jul 13 2023 15:06:43 GMT+0000 (Coordinated Universal Time)
cuid: clk1a9ly2000t09mq6ou1gv2f
slug: react-for-beginners-an-overview
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1689260257519/191dae4d-8039-4322-a9a0-2723ee4293fd.png
tags: tutorial, javascript, reactjs, beginners, frontend-development

---

Hello and welcome!!! 🤩🤩🤩🤩

This is the official last article of the complete [frontend web development series](https://dumebi.hashnode.dev/series/frontend-web-development). I am so excited to have come this far on this journey with you. It gives me great joy to see how much I have grown and how much you have all grown in these past three months. Thank you for sticking with me through this journey. I do not take the commitment and enthusiasm for granted.

In today's lesson, we will be talking about a very popular Javascript framework: React.

## Javascript Frameworks

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689173968235/d727fdf9-609b-4baa-8866-73135ac1cc0f.jpeg align="center")

***In a nutshell, JavaScript frameworks are collections of JavaScript libraries that contain JavaScript code, making life much easier for software developers. Each JavaScript framework provides pre-built scripts for many regions and purposes in software development, saving the developer time.***

### The Best Javascript Frameworks in 2023

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689175042305/abec045d-03fc-4636-9c53-b43696089e79.jpeg align="center")

There are a lot of Javascript frameworks, for various things. There are frameworks for front-end web development, back-end development, machine learning and AI, and more. There are currently about 83 Javascript frameworks in 2023.

We will talk briefly about a few of the frameworks used for front-end web development, and then turn our full attention to the most popular Javascript framework: React.

* [AngularJs](https://angularjs.org/): AngularJS is a discontinued free and open-source JavaScript-based web framework for developing single-page applications. It was maintained mainly by Google and a community of individuals and corporations.
    
* [Vue.js](https://vuejs.org/): Vue.js is an open-source model–view–view-model front-end JavaScript framework for building user interfaces and single-page applications. It was created by Evan You and is maintained by him and the rest of the active core team members.
    
* [Svelte](https://svelte.dev/): Svelte is a free and open-source front-end component framework or language created by Rich Harris and maintained by the Svelte core team members.
    
* [Ember.js](https://emberjs.com/): Ember.js is an open-source JavaScript web framework that utilizes a component-service pattern. It allows developers to create scalable single-page web applications by incorporating common idioms, best practices, and patterns from other single-page-app ecosystem patterns into the framework.
    

## React

React is a free and open-source front-end JavaScript library for building user interfaces based on components. It is maintained by Meta and a community of individual developers and companies. React can be used to develop single-page, mobile, or server-rendered applications with frameworks like Next.js.

### Getting started with React

The first place to go to get started with React is the [new React official documentation](http://react.dev).

### CRA or not?

To get started with React on our local IDEs, we will have to install React. Now, there are various ways to install a React app, but we will be looking at two methods: [CRA](http://react.dev), and [Vite](https://vitejs.dev/guide/).

### CRA

CRA is an acronym that stands for Create React App.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689180431221/1ddbdb63-818b-4baf-bc68-5e73279d2458.png align="center")

In the image above are the methods with which to initialize a react app on your local IDE.

* On your local IDE, create a folder in which to initialize your react project.
    
* On your terminal, enter any of the commands in the image above: npx, npm, or yarn. It should spin up a loading page like this. **Note: the image below is from the windows command terminal, and not that of a local IDE. It follows the same process nonetheless.**
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689230049186/2b34d382-fb18-4004-8fae-fcd597e078ac.jpeg align="center")
    
* After React has been installed; on your terminal, run the command
    
    `npm/npx/yarn start`
    
    It should spin up a page like the one below on your browser.
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689249499539/17a59ea7-18e9-46ed-aa15-c805b53288f5.webp align="center")
    

### Vite

Vite is a local development server written by Evan You and used by default by Vue and for React project templates. It has support for TypeScript and JSX.

Just like with CRA, we use Vite on the terminal.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1689252124970/c17a973f-2c40-4fe8-83b1-091e01a02588.png align="center")

For this tutorial, we will be using [code sandbox](http://codesandbox.io) as our cloud IDE.

### Functional components

For the most part, react code is written within a functional component.

***A React functional component is a simple JavaScript function that accepts props and returns a React element. After the introduction of React Hooks, writing functional components has become the ​standard way of writing React components in modern applications.***

How to separate a functional component from a normal function is that the first letter of the function name is capitalized, just like in a [constructor function](https://rollbar.com/blog/javascript-constructors/#:~:text=A%20constructor%20is%20a%20special,for%20any%20existing%20object%20properties.). However, a constructor function and a react function are not the same thing.

### JSX

***JSX stands for “JavaScript XML,” and it is a syntax extension to JavaScript based on ES6, the newest “version” of JavaScript. JSX allows you to write HTML in React by converting HTML into React components, helping you to create user interfaces for your web applications.***

<iframe src="https://codesandbox.io/embed/relaxed-franklin-mv8rng?fontsize=14&theme=dark" style="width:100%;height:500px;border:0;border-radius:4px;overflow:hidden" sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"></iframe>

See the sandbox above? You're probably asking, "Is that HTML inside javascript?" Well, that is JSX, javascript's markup language syntax. Keep in mind that JSX obeys the same principle as HTML, so whatever element is available in HTML is available in JSX, attributes as well. However, if you notice on the line that had the `div`, you will see that instead of `class`, we had `className`. Yes, that is because the word `class` is a [reserved keyword](https://www.w3schools.com/js/js_reserved.asp) in javascript. Although if you had written just `class`, your code would still run. This isn't a recommended practice.

For HTML attributes that are compound words, we use the camel notation to write them.

`export default function App()` is an example of a functional component. Notice how the function name app has its first letter capitalized.

There is something else new that we notice right?

The beauty of React is that it lets us build reusable components. Reusable in that we can have a component that contains pieces of code that we might want to use over and over again through the course of writing our app.

Think of it as storing a value in a variable. A value that you plan on reusing through your entire code, but you aren't willing to be writing it out every time you need it.

See that `Greetings` is our reusable component. At any point in writing our application, we can call on `Greetings`.

Notice the syntax in which it was written in `<Greetings />`, this is the syntax to introduce a new component.

Note:

1. We can have our components in different files asides from our App.js. We just have to create a new file in the src directory. If you are building a big application that has multiple components, it is advised to create a folder to group all your components to make your workplace clean.
    
2. `App.js` (`main.js` in a Vite app) is the main component of a React app. It is from here that we feed the React app what it should display.
    

### React Hooks

Hooks allow function components to have access to state and other React features.

They basically allow us to "hook" into React features.

You must `import` Hooks from `react`.

In the following example, we will use the `useState` Hook to keep track of the application state.

State generally refers to application data or properties that need to be tracked.

There are three rules for hooks:

* Hooks can only be called inside React function components.
    
* Hooks can only be called at the top level of a component.
    

I talk more about React Hooks in this [article](https://dumebi.hashnode.dev/react-hooks-explained).

### React useState Hook

The React `useState` Hook allows us to track state in a function component.

State generally refers to data or properties that need to be tracking in an application.

To use the `useState` Hook, we first need to `import` it into our component.

At the top of your component, `import` the `useState` Hook.

```jsx
import { useState } from "react";
function Example() {
const [state, updateState] = useState('Happy') //This is the general syntax for writing our useState
return(
<div>
</div>
)}
```

We initialize our state by calling `useState` in our function component.

`useState` accepts an initial state and returns two values:

* The current state.
    
* A function that updates the state.
    

Notice that we are destructuring the returned values from `useState`.

The first value, `state`, is our current state.

The second value, `updateState`, is the function that is used to update our state.

These names in our destructured array are variables that can be named anything you would like.

### Building a simple counter app with React

<iframe src="https://codesandbox.io/embed/misty-breeze-ct5fp6?fontsize=14&hidenavigation=1&theme=dark" style="width:100%;height:500px;border:0;border-radius:4px;overflow:hidden" sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"></iframe>

Above, we have a simple counter app that encompasses all that we have learned so far about React. Like was said earlier, the useState hook is used to manage the state of our react app at any given time.

Following this logic, we see that the state our app was in at the time of writing the code was 0. Keep in mind that our state can be any data type: number, string, boolean, object, or array. In the example we have, our state count is at 0. However, we want to be increasing this number without having to refresh our page every time we increase it. That is what the second part of our destructured array, `updateCounter`, is looking to do. `updateCounter` takes in a code block of what we want to happen to our state.

We put updateCounter in a function so as to add it to our button's onClick function.

I am so excited!!!!!! 🥳🥳🥳🥳

We are finally and officially at the end of our 12 days Frotnend web development series. I couldn't be prouder of each of you for taking this step and getting here.

***I urge each of you to, however, make sure that you do not stop your learning with these tutorials. There is still so much to be learned and explained. Watch as much videos as you can, and be sure to always read documentation. I am always here incase you have questions to ask.***

Cheers!

### References

[Cover Image](https://www.freecodecamp.org/news/react-js-for-beginners-props-state-explained/)

[Javascript frameworks](https://codeinstitute.net/global/blog/javascript-framework/#:~:text=In%20brief%2C%20JavaScript%20frameworks%20are,saving%20time%20for%20the%20developer.)

[Image: Javascript frameworks](https://amoniac.eu/blog/post/most-popular-js-frameworks-overview)

[Image: Best Javascript frameworks](https://jelvix.com/blog/best-javascript-frameworks)

[Image: React installation](https://www.techomoro.com/how-to-install-and-setup-a-react-app-on-windows-10/)

[Image: React start page](https://www.sitepoint.com/getting-started-react-beginners-guide/)

[What is JSX](https://egghead.io/learn/react/beginners/wtf-is-jsx#:~:text=JSX%20stands%20for%20%E2%80%9CJavaScript%20XML,interfaces%20for%20your%20web%20applications.)

[React Hooks](https://www.w3schools.com/react/react_hooks.asp)

[React useState](https://www.w3schools.com/react/react_usestate.asp)