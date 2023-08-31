---
title: "👌Setting up React Router v6 in your React app"
datePublished: Thu Aug 31 2023 20:47:19 GMT+0000 (Coordinated Universal Time)
cuid: cllzn0ctt000209l5cmhv9y1a
slug: setting-up-react-router-v6-in-your-react-app
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1693514667332/d6d4c124-7eb8-4de4-964e-3348b0c947cc.png
tags: javascript, web-development, router, reactjs, frontend-development

---

Are you tired of clunky, multi-page applications? Say hello to dynamic, single-page masterpieces with the React Router library. With React Router v6, things are about to get even better. This innovative update brings a component-based approach that aligns perfectly with React's philosophy, making it easier than ever to define routes, nested routes, and route transitions. Follow this guide to learn how to set up React Router v6 in your React app. Get ready to take your navigation experience to the next level.

## Setting up a React application

You must set up a React application to get started with React Router and add dynamic page routing to your development experience.

### Step 1

Create a directory from your terminal or through your GUI where you want your React app to be located.

On a terminal:

`mkdir React-app`

### Step 2

Write into the new folder you created.

On a terminal:

`cd React-app`

### Step 3

Using `create-react-app`, let us initialize a React application. There are other ways to initialize a React application that you can find [here](https://react.dev/).

On your terminal:

`npx create-react-app myApp`

After your app has been installed, you will find a message like this on your terminal.

***Please note that you will not find this exact message as the file names are different.***

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1693510218015/84ef4611-e605-488a-bde9-0d140a30e580.png align="center")

## Add React Router to your application

### Step 1

Write into the React app you just initialized.

`cd myApp`

### Step 2

Install React Router

On the terminal (make sure you are in the directory of your new app--myApp):

`npm install react-router-dom`

## Starting your React app

Finally, on your terminal:

`npm start`

This will spin up your React app in your browser on the local host 3000. You get something like this

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1693511633849/d58322e8-93f0-48d2-8a86-178f3cf97085.png align="center")

## Setting up React Router in your application

### Step 1

Open the directory of your app in VS Code. Your directory should look like this when opened in VS Code

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1693511923237/ab2c26c4-258c-4b18-87a0-ad1c9177fa11.png align="center")

### Step 2

In `App.js`, we will be importing from the `react-router-dom` module that we just installed.

`import { createBrowserRouter, RouterProvider} from 'react-router-dom';`

Importing this will enable us to create a path for our routes.

Still in `App.js`,

```javascript
import { createBrowserRouter, RouterProvider} from 'react-router-dom';

const router = createBrowserRouter([]) //Created a path for our individual routes

function App() {

  return (
    <RouterProvider router={router} /> //wrapped our component(s) in the React router provider.
  );
}
```

### Add routes

To properly use React router, our React app ought to have at least two pages/components that we will route between.

### Step 1

We will create two components that will be routed to each other. `PageOne` will route to `PageTwo`.

To create the components, left-click on the `src` folder and select `create new file`. This will be called

`PageOne.jsx`

Do the same for `PageTwo.jsx`

In the PageOne component:

```javascript
export default function PageOne() {
  return(
    <div>
      <button>Take me to page 2!</button>
    </div> )}
```

`PageTwo.jsx:`

```javascript
export default function PageTwo() {
  return(
   <div>
    <h1> Hello! This is page 2! </h1>
   </div>)}
```

### Step 2

Now that we have created our two components, we need to go back to the `PageOne.jsx` component, to link it to `PageTwo.jsx`.

We will be doing this by importing a property of `react-router-dom` named `Link`.

Having imported `Link`, it will be wrapped around the button element.

`Link` takes a `to` attribute that specifies where the element is linking to.

```javascript
import { Link } from "react-router-dom";

export default function PageOne() {
  return(
    <div>
      <Link to={'/pageTwo'}><button>Take me to page 2!</button></Link>
    </div> )}
```

### Step 3

The final step in this process is to go back to `App.js` and add this new route that was just created.

```javascript
import { createBrowserRouter, RouterProvider} from 'react-router-dom';

const router = createBrowserRouter([
  { 
    path: 'pageTwo',
    element: <PageTwo />
  }
]) //added a path for our route

function App() {

  return (
    <RouterProvider router={router} /> //wrapped our component(s) in the React router provider.
  );
}
```

And with that, when the button in `PageOne.jsx` is clicked, it takes us straight to `PageTwo.jsx`.

**Note that as many routes as required for your React app can be created and added to the path.** `router` **is an array, and therefore each route should be separated by a comma.**

## Conclusion

By implementing React Router v6 in your React app, you'll be able to create a sleek and effective navigation system that will enhance the user experience. The simplified API and component-based methodology of React Router v6 complement the fundamental principles of React development, setting you up for success. With the knowledge gained from this guide, you'll be prepared to install, define routes, and navigate between views using the most current version of React Router. As you delve deeper into the more advanced features and possibilities, you'll be fully equipped to build dynamic and engrossing single-page applications that will captivate your users.

## References

[CRA directory structure](https://www.google.com/url?sa=i&url=https%3A%2F%2Fmedium.com%2Fswlh%2Fdemystifying-the-folder-structure-of-a-react-app-c60b29d90836&psig=AOvVaw3fMq4K5an0-kBUG66joPZ6&ust=1693598131816000&source=images&cd=vfe&opi=89978449&ved=0CBAQjRxqFwoTCLjKiO3Wh4EDFQAAAAAdAAAAABAE)

[CRA page view](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.javatpoint.com%2Freact-create-react-app&psig=AOvVaw1TrLEPcHWuY1cNhrzJrYAl&ust=1693596270360000&source=images&cd=vfe&opi=89978449&ved=0CBIQjhxqFwoTCIj7nJjhh4EDFQAAAAAdAAAAABAE)

[CRA success page](https://www.google.com/url?sa=i&url=https%3A%2F%2Fvegibit.com%2Fcreate-react-app-tutorial%2F&psig=AOvVaw1TrLEPcHWuY1cNhrzJrYAl&ust=1693596270360000&source=images&cd=vfe&opi=89978449&ved=0CBAQjRxqFwoTCIj7nJjhh4EDFQAAAAAdAAAAABAJ)

[Cover image](https://www.google.com/url?sa=i&url=https%3A%2F%2Freactrouter.com%2F&psig=AOvVaw11s2j3VpvBwoXfHOVtyDnA&ust=1693600987897000&source=images&cd=vfe&opi=89978449&ved=0CBAQjRxqFwoTCICQlL7hh4EDFQAAAAAdAAAAABAJ)