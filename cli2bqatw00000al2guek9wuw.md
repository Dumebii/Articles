---
title: "What is an IDE? Best IDE to use for web development 2023"
seoTitle: "Learn how to choose an IDE for the best development experience"
seoDescription: "This article teaches how to set up a development environment. Different IDEs and their uses.  What IDE to choose when you start coding. comments"
datePublished: Sat May 06 2023 23:10:46 GMT+0000 (Coordinated Universal Time)
cuid: cli2bqatw00000al2guek9wuw
slug: learn-frontend-web-development-in-12days-setting-up-development-environment
cover: https://cdn.hashnode.com/res/hashnode/image/stock/unsplash/DuHKoV44prg/upload/4b7ac5d26c5f7bb7aa12d8e110033572.jpeg
tags: css, javascript, ides, web-development, html5

---

This is a side article to get you started with front-end web development.

## What are IDEs?

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1684969978999/8200b282-0aba-490a-a817-2a3fcc43d6a7.png align="center")

***An integrated development environment (IDE) is a software tool that assists programmers in effectively producing software code. It boosts developer productivity by merging features like software editing, building, testing, and packaging into a single, user-friendly tool. Software engineers, like authors, use text editors, and accountants use spreadsheets to make their jobs easier.***

To write code, you can use any text editor. However, most integrated development environments (IDEs) provide features other than text editing. They provide a centralized interface for commonly used developer tools, making the software development process much more efficient. Instead of manually integrating and configuring various software, developers may begin programming new applications immediately. They also do not need to learn about all the tools and can concentrate on just one application.

### Local IDEs

IDEs for local use Developers install and operate local IDEs on their computers. In addition, depending on their coding tastes, project requirements, and development language, they must download and install numerous extra libraries. Local IDEs are customizable and, once installed, do not require an online connection. Some examples of local IDEs used for web development include

* **VS Code**: Visual Studio Code, also commonly called VS Code, is a source-code editor made by Microsoft with the Electron Framework, for Windows, Linux, and macOS.
    
* **Atom**: Atom is a deprecated free and open-source text and source code editor for macOS, Linux, and Windows with support for plug-ins written in JavaScript, and embedded Git Control.
    
* **Sublime Text:** Sublime Text is a shareware text and source code editor available for Windows, macOS, and Linux. It natively supports many programming languages and markup languages.
    

### Cloud IDEs

Developers use cloud IDEs to write, edit, and compile code directly in the browser so that they don't need to download software on their local machines. Cloud-based IDEs have several advantages over traditional IDEs. Examples of cloud IDEs include:

* [CodePen](http://codepen.io): CodePen is an online community for testing and showcasing user-created HTML, CSS, and JavaScript code snippets. It functions as an online code editor and open-source learning environment, where developers can create code snippets, called "pens," and test them.
    
* [Codeply](http://www.codeply.com): Codeply is the HTML, CSS, and JS editor that makes frontend design and development easier by enabling you to leverage the frameworks of your choice.
    
* [CodeSandBox](http://codesandbox.io): ***CodeSandbox*** is a cloud development platform that empowers developers to code, collaborate, and ship projects of any size from any device in record time.
    

For this tutorial, we will be using CodePen for our coding examples and results.

## Comments

Comments are specially marked lines of text in the program that are **not evaluated**. There are usually two syntactic ways to comment. The first is called a *single-line comment* and, as implied, only applies to a single line in the "source code" (the program). The second is called a *Block* comment and refers usually refers to a paragraph of text. A block comment has a start symbol and an end symbol and everything between is ignored by the computer.

```xml
<p> I am a girl </p>
<!-- this is a comment syntax in HTML -->
```

```css
body {
background-color: green;
}
/* This is a comment syntax in CSS */
```

```javascript
var name = "Dumebi";
// This is a comment syntax in javavscript.
```

## Setting up HTML

Every HTML document ends with the extension `.html` .

Although we will be using a cloud IDE in this tutorial, you can also join in with your local IDE.

In your local computer, create a file with the extension '`.html`' and loading it up on any local IDE of your choice will lead you straight into the HTML development environment.

### HTML Boilerplate

```xml
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>HTML 5 Boilerplate</title>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
	<script src="index.js"></script>
  </body>
</html>
```

This HTML boilerplate should be the first set of code you have down in your HTML file. [Learn more about the HTML boilerplate here](https://www.freecodecamp.org/news/basic-html5-template-boilerplate-code-example/)

With this boilerplate down, you can begin writing your code in HTML.

Some local IDEs like Atom have shortcuts that automatically load up this boilerplate for any `.html` file.

## Setting up your CSS

CSS files end with the extension `.css`. There are three ways of writing CSS, which would be discussed more in-depth when we get to the section on CSS. For now, I'd show you how to link a CSS file to an HTML file.

```xml
<link rel="stylesheet" href="style.css">
```

In the HTML boilerplate shared above, we can see this line of code embedded in it. This is how to link a CSS file in HTML, by first opening a `<link>` tag. The link tag has an attribute `rel` meaning relationship. We see that the relationship here is that the CSS file is a `stylesheet`. It has another attribute `href`. `Href` attributes are used to link files/websites in HTML. This wouldn't make much sense right now until we have covered the introduction to the HTML article. Don't bother yourself trying to understand it all. But this gives a very good foundation for when we start learning.

***To enable this linking, the HTML file, and the CSS file have to be in the same hierarchy in the saving system.***

***Read more about file hierarchy*** [***here***](https://www.easytechjunkie.com/what-is-a-hierarchical-file-system.htm)

## Setting up the Javascript

```xml
<head>
<!--Insert boilerplate code here-->
</head>
<body>
   <script src="index.js"></script>
</body>
```

Similar to setting up our CSS, we set up our javascript embedded in a `script` tag. Now, unlike our CSS that we see is placed above our `body` tag, we can initially see that our `script` tag is placed in between (usually at the end of our entire HTML code) our `body` tag. This is the best practice behavior that will be explained better when we begin to learn our javascript.

However, there is another way to place our script tag in an HTML document.

```xml
<head>
<script src='index.js' async></script>
<!--<script src='index.js' async></script>-->
</head>
```

We can see in the above example, that our `script` tag is embedded in our `head` element, this is because two keywords are associated with the `script` tag. The `await` and `async` keywords. We will talk more about this in our javascript class. It will more sense as the classes go by. Javascript files are written with the extension `.js`.

***To enable this linking, the HTML file, and the javascript file have to be in the same hierarchy in the saving system.***

***Read more about file hierarchy*** [***here***](https://www.easytechjunkie.com/what-is-a-hierarchical-file-system.htm)

For our cloud IDEs, however, we do not need to go through this entire process as everything has been automated for easy usage and retrieval. The above explanations are for those who will be following this class with a local IDE.

## References

[Seven best IDEs for javascript](https://www.tabnine.com/blog/best-ides-for-javascript/)

[What is an IDE](https://aws.amazon.com/what-is/ide/#:~:text=An%20integrated%20development%20environment%20(IDE,easy%2Dto%2Duse%20application)

[HTML boilerplate](https://www.freecodecamp.org/news/basic-html5-template-boilerplate-code-example/)

[Comments](https://users.cs.utah.edu/~germain/PPS/Topics/commenting.html)