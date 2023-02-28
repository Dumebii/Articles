# Building your first server with ExpressJs

Hello and Welcome!! 🤩🤩🤩

I am super excited to write this article, and I hope you have as much fun reading it as I did writing it.

To begin with, let us understand what ExpressJs is.

*Express.js, or simply Express, is a back-end web application framework for building RESTful APIs with Node.js, released as free and open-source software under the MIT License. It is designed for building web applications and APIs. It has been called the de facto standard server framework for Node.js.* [source](https://en.wikipedia.org/wiki/Express.js)

Knowing now that Express is a NodeJs framework. We will be relying a lot on the use of NodeJs, especially for the installation of Express.

### *Installing Hyper Terminal*

Please note that it is completely okay to use your Os' inbuilt command terminal. I prefer using Hyper Terminal, and that is what I'd be using throughout this article.

A guide on how to download and install the hyper terminal can be found on their documentation page [here](https://hyper.is/#installation)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1677525619671/0bdce0db-32ad-4193-99fa-e8e730d74ea7.png align="center")

### *Installing NodeJs.*

![Nodejs installation page with windows highlighted](https://cdn.hashnode.com/res/hashnode/image/upload/v1677523795483/066b6cef-a6c7-4372-8238-6195455be3ff.png align="center")

This is a preliminary step to achieve our goal as we will be needing a feature of Nodejs, which is its package manager, NPM (**Node Package Manager**). A complete guide on how to install and set up Node on your computer can be found on the documentation page [here](https://nodejs.org/en/download/). Choose which OS you use, and follow the prompts as you go. I use a windows laptop, and that's why the windows installer is highlighted. 😅😅

### *Creating your first Express server*

Having finished the first two steps, it is time for us to get right into it!!

1. On your hyper terminal, you create a new directory on your desktop with the following command
    
    `mkdir express file`
    
2. Go ahead to create a new file inside this directory by using the following command.
    
    `touch server.js`
    
3. Still, in the same directory, we run `npm init` and follow the prompts where necessary.
    
4. For the purpose of this tutorial, I am using the Atom code editor. To open up our `server.js` file in Atom: we, still in the same directory, use this command `atom .`
    
5. The next step is to install ExpressJs. From the [documentation](https://expressjs.com/en/starter/installing.html), we see that all we have to do is run this command `npm install express` in our terminal (still in the same directory). This installs the Express package onto our local computer.
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1677525484182/49ca6be6-648b-4f6e-8c95-7f9660e1eba3.jpeg align="center")
    
6. After this is done, we can go ahead to create our first server!!! 💃🏾💃🏾💃🏾
    
    In our code area, we type in the following...Don't worry, I'd explain.
    
    ```javascript
    //jshint esversion:6
    
    const express = require('express');
    
    const app = express();
    
    app.listen(3000);
    ```
    

* Our first line of code is a comment (that is specific to Atom), telling Atom that we are using ES6 so that it doesn't shoot a bunch of errors at us.
    
* The next line is us *requiring Express.* That is*, fetching Express.* We store this in a `const.`
    
* The next line is fetching the Express module or method, and storing it in a `const` named 'app'.
    
* The last line is us calling a property of the `express` method, 'listen', to listen on port 3000. This simply means that we are creating a (local) server on port 3000.
    

### *Starting up your server*

Back in our terminal, we enter the command `node server.js`. This starts up our server. We will know that this is successful when, after executing the command, our terminal ceases to generate the usual prompts for us. This indicates that the server is on.

We can, however, go a step further by adding an anonymous function to our listen property.

```javascript
//jshint esversion:6

const express = require('express');

const app = express();

app.listen(3000, funtion(){
console.log('THe server has started on port 3000')};
```

You will see this spin-up on your terminal window when you start the server. This shows you that your server has started running.

*To exit the server on the terminal, type* `ctrl + c` *or* `cmd + c`*.*

There you have it, your very first server!

There are lots and lots of cool and interesting things that we will be doing with Express going forward, but that is all for this article. Catch you next time!