---
title: "Learn Frontend web development in 12 days"
seoTitle: "Learn web development in 12 days HTML development 
Beginner web devel"
seoDescription: "Learn beginner HTML, Learn HTML for beginners, basics of HTML, how to learn web development, beginning web development with HTML."
datePublished: Wed May 10 2023 13:30:39 GMT+0000 (Coordinated Universal Time)
cuid: clhhqnjp8001q8inv8qn3ewlb
slug: learn-frontend-web-development-in-12-days-1
cover: https://cdn.hashnode.com/res/hashnode/image/stock/unsplash/wUbNvDTsOIc/upload/0eeae6a56195b5b4d38281c14191180b.jpeg
tags: tutorial, web-development, html5, beginners, semantichtml

---

Hello, and welcome back!! 😁😁

## Introduction

Today, we are going straight into the heart of web development. I consider HTML the heart of web development because there isn't a website without HTML.

In the era before CSS and Javascript became a thing, people would write (and design) entire websites with just HTML. This is to learn and understand web development, especially the front-end, you need to know HTML.

HTML stands for Hypertext Markup Language.

## Definition

***HTML (Hypertext Markup Language) is the standard language used to create web pages. HTML provides the structure and content of a web page and is used to define the different elements of a page, such as headings, paragraphs, images, and links. In this introductory lesson, we will cover the basics of HTML and how to create a simple web page.***

## Definition of terms

Here's a sample HTML page I built using just HTML. It was meant to be a portfolio website [Portfolio](https://dumebii.github.io/cv/)

1. ### Elements:
    
    The HTML **element** is everything from the start tag to the end tag:
    
    `<tagname>Content goes here...</tagname>`
    
    Examples:
    
    ```xml
    <header>This is the Header</header>
    
    <main>This is the main section of the website</main>
    
    <article>Hi. I am a written long paragraph!</article>
    
    <div>Hi. I am a container!!</div>
    ```
    
    <iframe height="248" style="width:100%" src="https://codepen.io/dumebii/embed/VwEQqae?default-tab=html%2Cresult">
      See the Pen <a href="https://codepen.io/dumebii/pen/VwEQqae">
      Untitled</a> by Dumebi Okolo (<a href="https://codepen.io/dumebii">@dumebii</a>)
      on <a href="https://codepen.io">CodePen</a>.
    </iframe>
    
    * ### Nested HTML Elements
        
        HTML elements can be nested (this means that elements can contain other elements).
        
        All HTML documents consist of nested HTML elements. An example of a nested element can be
        
        `<h1>This is a <em> major </em> heading </h1>`
        
        In this example, we see that the `<em>` is embedded into the `<h1>` tag. The `<em>` tag is used to emphasize part/parts of a text.
        
    
    ### Attributes
    
    HTML attributes provide additional information about HTML elements. They are embedded into the opening tag of an element.
    
    * All HTML elements can have **attributes**
        
    * Attributes provide **additional information** about elements
        
    * Attributes are always specified in **the start tag**
        
    * Attributes usually come in name/value pairs like **name="value"**
        
        Example:
        
        `<h1 id="heading-1"> Hi! I am the largest heading </h1>`
        
    
    ### Tags
    
    HTML tags are like keywords that define how a web browser will format and display content. With the help of tags, a web browser can distinguish between HTML content and simple content. HTML tags contain three main parts: opening tag, content, and closing tag. But some HTML tags are unclosed.
    
    * All HTML tags must be enclosed within &lt; &gt; these brackets.
        
    * Tags in HTML perform different tasks.
        
    * If you have used an open tag `<tag>`, then you must use a close tag `</tag>` (except for some tags that are self-closing as such: `<br/>`)
        
        ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1683549118523/c98fe428-cb52-460d-b407-c3834c5ee264.png align="center")
        
    
    ### Block and Inline elements:
    
    Every HTML element has a default display value, depending on what type of element it is.
    
    There are two display values: block and inline.
    
    * **Block elements**: A block-level element always starts on a new line, and the browsers automatically add some space (a margin) before and after the element.
        
        A block-level element always takes up the full width available (stretches out to the left and right as far as it can).
        
    * **Inline elements:** An inline element does not start on a new line.
        
        An inline element only takes up as much width as necessary.
        
    

## Semantic HTML

Before we get started properly, there is a concept in HTML I will like to introduce.

Semantic HTML is the practice of using HTML elements to convey meaning and structure to the content of a web page, rather than just using them for presentation purposes. Semantic HTML helps search engines and assistive technologies (such as screen readers) understand the content and purpose of each element, which can improve the accessibility, usability, and search engine optimization (SEO) of a web page.

Some examples of semantic HTML elements include:

* `<header>`: Defines the header section of a page or section.
    
* `<nav>`: Defines a section of navigation links.
    
* `<main>`: Defines the main content area of a page.
    
* `<article>`: Defines a self-contained article or content block.
    
* `<section>`: Defines a section of related content.
    
* `<aside>`: Defines a section of content that is related to but separate from the main content.
    
* `<footer>`: Defines the footer section of a page or section.
    

By using semantic HTML, you can provide more context and meaning to the content of your web page, making it more accessible and understandable to users and search engines. This can also help with SEO by providing additional information to search engines about the content and structure of your page, which can improve its ranking in search results.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1683549322478/2a5335ee-c092-42bd-bb9f-3630b2ce6651.webp align="center")

## **HTML Document Structure**

An HTML document is composed of a series of elements, which are enclosed in tags. Tags are used to indicate the start and end of an element. The basic structure of an HTML document consists of the following:

```xml
<!DOCTYPE html>
<html>
  <head>
    <title>Page Title</title>
  </head>
  <body>
    <h1>Heading 1</h1>
    <p>Paragraph</p>
  </body>
</html>
```

* The `<!DOCTYPE html>` declaration defines the document type and must be included at the beginning of every HTML document.
    
* The `<html>` element is the root element of an HTML document.
    
* The `<head>` element contains meta information about the document, such as the title of the page.
    
* The `<title>` element specifies the title of the document, which is displayed in the browser's title bar.
    
* The `<body>` element contains the visible content of the web page.
    

## Conclusion

The key to learning HTML is learning as many elements as you can. I do not personally believe that a person can learn all the HTML elements available, but with foundational knowledge, you can always figure out what you are looking for.

In the next lesson, next week, we will take a deep dive into learning about different HTML elements, and their uses/functions. We will also be looking at HTML attributes.

Thank you so much for dropping in today and this week. Hope you have as much fun reading this as I did writing it.

Until next week, bye!! 🤩🤩🤩

## References:

[W3Schools](https://www.w3schools.com/html/default.asp)

[Java T Point](https://www.javatpoint.com/html-tags)

[Hackr blog](https://hackr.io/blog/html-projects)

[Semrush](https://www.semrush.com/blog/semantic-html5-guide/)

[My very trusty GPT 😅](https://chat.openai.com/)