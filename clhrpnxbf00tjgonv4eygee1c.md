---
title: "Learn Frontend Web development in 12 days!!"
seoTitle: "Learn core HTML principles// learn frontend development//"
seoDescription: "Learn core HTML principles// HTML accessibility// HTML attributes// Frontend web development// Web development// important HTML elements// HTML tags//"
datePublished: Wed May 17 2023 13:00:39 GMT+0000 (Coordinated Universal Time)
cuid: clhrpnxbf00tjgonv4eygee1c
slug: learn-frontend-web-development-in-12-days-1
cover: https://cdn.hashnode.com/res/hashnode/image/stock/unsplash/_t-l5FFH8VA/upload/cddafe04669dbd444b177a10bd9c56ca.jpeg
tags: tutorial, web-development, accessibility, html5, frontend-development

---

Hello and welcome to the third day of this series! 😃😃

It is so great to have you here.

Today, we will be picking up from where we stopped in the last lesson. We will be taking a deeper look into HTML (HyperText Markup Language), and how we can learn to be better web developers and HTML enthusiasts. We will also look at the core and necessary HTML elements.

## HTML Attributes

![An image showing HTML attributes](https://cdn.hashnode.com/res/hashnode/image/upload/v1684197667723/b8c8df5a-5a1c-493e-b02b-991f5367cc0e.jpeg align="center")

HTML attributes are an essential part of building web pages. They provide additional information about an HTML element, allowing developers to customize the appearance and behavior of web pages.

Example:

```xml
<h1 class='heading-1'> Hello! I am the largest heading! </h1>
```

In this syntax, `h1` is the HTML element to which the attribute is being added, `class` is the name of the attribute, and the value-pair, `class='heading-1'` refers to the value of the attribute. Some attributes, like `checked` or `selected`, do not require a value and are simply added as follows:

```xml
<input checked>This is a check box </input>
```

### HTML Attribute Types

HTML attributes are classified into two types: **global attributes** and **element-specific attributes.**

**Global attributes**: which include `class`, `id, style, and title,` can be added to any HTML element.

**Element-specific attributes:** these are properties that are unique to specific HTML elements. The `href` attribute, for example, is unique to anchor `<a>` elements, but the `src` attribute is unique to image `<img>` element.

### HTML Attributes in Common Use

HTML attributes are used to change the appearance and behavior of web pages in a variety of ways. Here are some examples of HTML properties in use:

**Styling**: CSS styles are applied to HTML components using attributes such as `class, id, and style`. We will be looking at CSS in our next class, and how we can use these attributes to effect changes to our webpage.

**Hyperlinks**: The `href` property is used to make links to other web pages or resources.

**Images**: The `src` attribute specifies the image's source file, whilst the `alt` attribute offers a description of the image for accessibility purposes.

**Forms**: `name` and `value` attributes are used to identify and give data for form elements such as input fields and buttons.

**Accessibility**: Screen attributes such as `title, aria-label,` and `aria-describedby` are utilized to convey additional information.

## HTML Accessibility

![An example of an accessible HTML snippet](https://cdn.hashnode.com/res/hashnode/image/upload/v1684197879558/68ccccf2-22ab-43ec-85d6-b7f87d5d610c.png align="center")

The topic of accessibility is rather peculiar to me, and that is because it is something that I haven't been able to learn properly. However, for the sake of inclusion and making sure people with disabilities are able to browse the Internet, the topic of accessibility must be emphasized, to ensure the message and importance is properly understood.

Accessibility has become an increasingly important topic, aiming to ensure that websites and web applications are usable and inclusive for all individuals, including those with disabilities.

**Semantic Markup:** Semantic HTML involves using the appropriate HTML elements to provide meaning and structure to web content. For example, using `<h1>` for headings, `<p>` for paragraphs, `<nav>` for navigation menus, and `<footer>` for the page footer helps create a well-structured document that is easily navigable.

HTML5 introduced landmark roles, which are specific HTML elements that define their purpose or role within the page. Landmark roles include `<header>`, `<nav>`, `<main>`, `<aside>`, `<article>`, `<footer>`, and `<section>`. These roles help screen readers and other assistive technologies understand the organization of the content, making it easier for users to navigate through the page and locate specific sections.

**Form Accessibility:** Forms are a common element on websites, and it is crucial to make them accessible. HTML provides attributes such as `label`, `fieldset`, and `legend` to associate labels with form controls, making them more understandable for screen readers. Additionally, providing clear instructions, using proper error messages, and utilizing HTML5 form validation attributes like `required` and `pattern` contribute to a more accessible form experience.

### ARIA in web development

Most developers are familiar with **HyperText Markup Language** (HTML), the standard markup language of the modern web. However, you may be less familiar with **Accessible Rich Internet Applications** (ARIA) (officially known as WAI-ARIA): what it is, how it is used, and when it should and should not be utilized.

HTML and ARIA play critical roles in making digital products accessible, particularly for assistive technology (AT) such as screen readers. Both are used to transform content into other formats like Braille or Text-to-Speech (TTS).

ARIA modifies incorrect or incomplete code to create a better experience for those using AT by changing, exposing, and augmenting parts of the accessibility tree.

ARIA does not affect an element's functionality or visual appearance on its own. That is, only AT users will perceive differences between a digital product that includes ARIA and one that does not. That also implies that developers must make the necessary code and stylistic adjustments to make an element as accessible as possible.

ARIA's three main components are roles, properties, and states/values.

```xml
<div role="button">Self-destruct</div>
<div role="button" aria-describedby="more-info">Self-destruct</div>
<div id="more-info">This page will self-destruct in 10 seconds.</div>
```

This section is an excerpt from this amazing article about ARIA in web development, and all you need to know about it. When to use ARIA in web development, and how to improve your web development journey for users with disabilities using screen readers or assistive devices... [ARIA in web development](https://web.dev/learn/accessibility/aria-html/)

## HTML Forms

An HTML form is used to collect user input.

<iframe height="402" style="width:100%" src="https://codepen.io/dumebii/embed/eYPLmdW?default-tab=html%2Cresult">
  See the Pen <a href="https://codepen.io/dumebii/pen/eYPLmdW">
  Untitled</a> by Dumebi Okolo (<a href="https://codepen.io/dumebii">@dumebii</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

In this HTML snippet, we see a very basic example of the HTML form element.

1. The `<label>` element is what produces the result "Enter your name". A Label element is used to label an input field. The `for` attribute in the label is to tell the HTML document what input element the label belongs to.
    
2. The `<input>` element is the *big empty* space for an input to be put in the results section.
    
3. The `type` attribute is to tell the browser exactly what input type of input it is to expect. It could be `text`, `number`, `email, date`, and so on. The `name` attribute is to associate it with the `label` element.
    
4. The `required` attribute is to tell the browser that the input field in question is a required field to be filled.
    
5. The `textarea` is another input type. Ordinarily, text areas in forms are used for large chunks of text like writing comments and so on. It has two attributes, the `rows`, and `cols` to determine the height and width of the text area.
    
6. The last three input fields are the `checkbox, radio button` and `submit` fields. We can see now how by changing the type of input field, we get a wide range of possibilities.
    
7. We see a `checked` attribute. This is just to precheck the button or box, that is, not giving the user the option to uncheck it. If we do remove the attribute, then the checking is up to the user.
    

## HTML Tables

HTML tables allow web developers to arrange data into rows and columns.

<iframe height="300" style="width:100%" src="https://codepen.io/dumebii/embed/NWOOKYv?default-tab=html%2Cresult">
  See the Pen <a href="https://codepen.io/dumebii/pen/NWOOKYv">
  Untitled</a> by Dumebi Okolo (<a href="https://codepen.io/dumebii">@dumebii</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

The above example shows the syntax for HTML tables. Of course, some tables can go longer, and get more complicated than this. Recently, HTML tables haven't been very popular in use, but they are still beneficial to learn, as you'd never know where or when they'd come in handy.

1. `<table>` element is what defines the table. This is what tells your browser that the display we are looking to get is that of a table.
    
2. `<thead>` element is used to affix a heading to the table.
    
3. The `<tr></tr>` simply put means table rows. It is used to show the browser the beginning and end of a particular set of values on the table. Tables are basically just a group of rows. In our example, the first `<tr></tr>` encapsulated the first set of rows, and so on.
    
4. `<td>` defines a cell in a table. That is, you enclose whatever data it is you want to be displayed on each call of the table in the `<td>` tag.
    

## HTML Lists

<iframe height="248" style="width:100%" src="https://codepen.io/dumebii/embed/MWPqRey?default-tab=html%2Cresult">
  See the Pen <a href="https://codepen.io/dumebii/pen/MWPqRey">
  Untitled</a> by Dumebi Okolo (<a href="https://codepen.io/dumebii">@dumebii</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

The above example is what is called an HTML list system.

1. The list enclosed in the `<ul>` tag comes out as bullet-point list items.
    
2. `<li>` simply means list items, and it is used to itemize data in a list.
    
3. `<ol>` stands for an ordered list, and is used to make an ordered list, that will have the list items arranged in order of ascending or descending numbers.
    

## Common/ Important HTML tags or elements

These elements are what you are likely to come across often or use as you continue down on your web development journey. The list of HTML tags is long, but these will surely get you in the right direction.

* `<a>` for link
    
* `<b>` to make bold text
    
* `<strong>` for bold text with emphasis
    
* `<body>` main HTML part
    
* `<br>` for break
    
* `<div>` it is a division or part of an HTML document
    
* `<h1>`...`<h6>` for titles/headings
    
* `<i>` to make an italic text
    
* `<img>` for images in the HTML document
    
* `<ol>` is an ordered list
    
* `<ul>` for an unordered list
    
* `<li>` is a list item in a bulleted (ordered list)
    
* `<p>` for a paragraph
    
* `<span>` to style part of a text
    
* `<header>` to define the heading of a website. There is usually only one header per website or page.
    
* `<footer>` to define the footer of a website or page.
    
* `<main>` This represents the main section of a page or website.
    
* `<section>` which defines a section of a website or page. You can have multiple sections across a website or page.
    

## Conclusion

***HTML is a very broad and long subject and is not one that can be exhausted in just two lessons. However, these lessons were to give you a guide and insight into what HTML is, the best practices for writing HTML, and how best to learn HTML for web development.***

I had so much fun writing this, and I hope you have a good time reading it as well!!

I will see you in our next class, where we take on the *almighty* CSS!! 😏😏

## References

[My very trusty GPT 😅😅](https://chat.openai.com/)

[MDN web docs on forms](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form)

[W3schools on HTML accessibility](https://www.w3schools.com/html/html_accessibility.asp)

[HTML attributes](http://web.simmons.edu/~grabiner/comm244/weekone/html-attributes.html)

[HTML accessibility](https://dev.to/njericooper/7-must-haves-for-html-in-your-site-template-578i)

[HTML tables](https://www.w3schools.com/html/html_tables.asp)

[Common HTML elements](https://www.codebrainer.com/blog/top-10-html-tags)