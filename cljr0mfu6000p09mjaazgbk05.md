---
title: "What is jQuery and why do you need to learn it?"
seoTitle: "jQuery. What is jQuery? Why should you learn jQuery? How to use jQuery"
seoDescription: "In this article,, we will be looking at what is jQuery? Why should you learn jQuery? How can you use jQuery for web development? Which companies use jQuery?"
datePublished: Thu Jul 06 2023 10:39:04 GMT+0000 (Coordinated Universal Time)
cuid: cljr0mfu6000p09mjaazgbk05
slug: what-is-jquery-and-why-do-you-need-to-learn-it
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1688639702161/6485e4a4-f561-4788-8a8b-2631b5f03ec7.png
tags: tutorial, jquery, javascript, web-development, dom-manipulation

---

Hello and welcome!! 🤩🤩🤩

We are slowly getting to the end of this series, and I am so excited! I hope you have had as much fun reading my articles as I have had writing them.

Today, we are taking a deep dive into jQuery, a popular Javascript library used for web development.

## What is jQuery?

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1688597654478/37028f2e-bda0-4ca3-894b-c89d4c6e2d14.jpeg align="center")

jQuery is a JavaScript [library](https://htschool.hindustantimes.com/editorsdesk/knowledge-vine/coding-library-what-is-it-all-about#:~:text=are%20coding%20libraries%3F-,Coding%20libraries%20are%20collections%20of%20pre%2Dwritten%20codes%20that%20are,to%20optimize%20their%20coding%20tasks.) designed to simplify HTML DOM tree traversal and manipulation, as well as event handling, CSS animation, and [Ajax](https://www.w3schools.com/xml/ajax_intro.asp). It is free, open-source software using the permissive MIT License. As of August 2022, jQuery was used by 77% of the 10 million most popular websites.

Basically, JQuery is to Javascript what Tailwind is to CSS in that it makes writing Javascript DOM manipulation codes shorter, cleaner, and more efficient.

## Why should you learn jQuery?

jQuery takes a lot of everyday tasks that require many lines of JavaScript code to accomplish and wraps them into methods that you can call with a single line of code. There are lots of other JavaScript libraries out there, but jQuery is probably the most popular, and also the most extendable.

## How to add jQuery to your HTML

Before you start using jQuery, you need to get it on your local IDE.

There are two ways to get jQuery

1. **Downloading**: jQuery is registered as [a package](https://www.npmjs.com/package/jquery) on [npm](https://www.npmjs.com/). You can install the latest version of jQuery on your terminal with the npm CLI command:
    
    `npm install jquery`
    
    As an alternative, you can use the [Yarn](https://github.com/yarnpkg/yarn) CLI command:
    
    `yarn add jquery`
    
    This will install jQuery in the `node_modules` directory.
    
    Within `node_modules/jquery/dist/` you will find an uncompressed release, a compressed release, and a map file.
    
    You can learn more about this download and other methods of downloading on the jQuery [official documentation page](https://jquery.com/download/).
    
2. **Through a CDN**: in our [lesson](https://dumebi.hashnode.dev/learn-frontend-development-in-12-days-css-frameworks), we talked about what a CDN is and how we can use it to download libraries and frameworks on to our local IDEs.
    
    To use the jQuery CDN, just reference the file in the script tag directly from the jQuery CDN domain. You can get the complete script tag, including *Subresource Integrity attribute*, by visiting [here](https://releases.jquery.com) and clicking on the version of the file that you want to use. Copy and paste that tag into your HTML file.
    
    The following CDNs also host compressed and uncompressed versions of jQuery releases. Starting with jQuery 1.9 they may also host [sourcemap files](https://blog.jquery.com/2013/01/09/jquery-1-9-rc1-and-migrate-rc1-released/#sourcemaps); check the site's documentation.
    
    ***Note that there may be delays between a jQuery release and its availability there. Please be patient; they receive the files at the same time the blog post is made public. Beta and release candidates are not hosted by these CDNs.***
    
    * [Google CDN](https://developers.google.com/speed/libraries#jquery)
        
    * [Microsoft CDN](https://learn.microsoft.com/en-us/aspnet/ajax/cdn/overview#jQuery_Releases_on_the_CDN_0)
        
    * [CDNJS CDN](https://cdnjs.com/libraries/jquery/)
        
    * [jsDelivr CDN](https://www.jsdelivr.com/package/npm/jquery)
        

jQuery provides several methods to manipulate the DOM efficiently. You do not need to write big and complex code to set or get the content of any HTML element.

## **jQuery DOM Manipulation**

jQuery provides methods such as `attr()`, `html()`, `text()` and `val()` which act as getters and setters to manipulate the content of HTML documents.

### Basic jQuery DOM commands

1. Unlike in javascript [DOM manipulation](https://dumebi.hashnode.dev/javascript-dom-manipulation-the-document-object-model) where we have
    
    `document.querySelector("css-selector")` as the way to target HTML elements, with jQuery, all we need is a dollar sign '$'. So, the initial example becomes
    
    `$('css-selector')`
    
    ```javascript
    $('h1')
    //this is the basis syntax of a jQuery DOM manipulation code
    ```
    
2. To change any CSS style, we use the `css` method in the following syntax:
    
    `$('css-selector').css('css-property','property-value')`
    
3. To target (modify) only the text of an HTML element:
    
    `$('css-selector).text("This is a new text!")`
    
4. To target (modify) the text in an HTML element or to add a child element:
    
    `$('css-selector').html("<en> Kiss me! </en>")`
    
5. To set an attribute:
    
    `$('css-selector').attr("attribute-type", "attribute-name")`
    
6. To add or remove a class:
    
    `$('css-selector').addClass("new-class")`
    
    `$('css-selector').removeClass("old-class")`
    
7. To add multiple classes:
    
    `$('css-selector').addClass("new-class new-class")`
    
8. To add an event listener:
    
    `$('css-selector').event(function(){--this is a function block--})`
    
9. We can also add HTML elements to already existing elements, depending on where we want them:
    
    `$('css-selector').before("element to be added")` This adds the new element before the selected element.
    
    `$('css-selector').after("element to be added")` This adds the new element after the selected element.
    
    `$('css-selector').prepend("element to be added")` This adds the new element besides the selected element to the left.
    
    `$('css-selector').append("element to be added")` This adds the new element besides the selected element to the right.
    

Here is an example of using all we have learnt in one document:

<iframe height="264" style="width:100%" src="https://codepen.io/dumebii/embed/yLQorGx?default-tab=js%2Cresult">
  See the Pen <a href="https://codepen.io/dumebii/pen/yLQorGx">
  Untitled</a> by Dumebi Okolo (<a href="https://codepen.io/dumebii">@dumebii</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

You can also check out this github [repo](https://github.com/Dumebii/Simon-Game/blob/main/game.js) dealing how to build the Simon Game with jQuery.

That's all for today, guys!

I am so glad that I got to teach jQuery to you all. A lot of people will tell you that learning jQuery is not important to modern-day developers. Well, I disagree. I think learning jQuery helps solidify your foundation as a badass Javascript developer. Also, companies still ask for jQuery as a skill to be had for employment.

See you all next week!!

## References

[Image: What is jQuery?](https://slideplayer.com/slide/12409003/)

[jQuery HTML DOM Manipulation](https://www.tutorialspoint.com/jquery/jquery-dom.htm#)

[Cover photo](https://hackr.io/blog/what-is-jquery)