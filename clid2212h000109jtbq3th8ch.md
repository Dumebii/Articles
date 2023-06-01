---
title: "Learn Frontend Web Development in 12 days!!!"
seoTitle: "Advanced CSS concepts media queries CSS blend modes"
seoDescription: "Advanced CSS concepts media queries CSS blend modes css variables css flexbox css grid css positions responsive design. good css practice. example css"
datePublished: Thu Jun 01 2023 11:30:42 GMT+0000 (Coordinated Universal Time)
cuid: clid2212h000109jtbq3th8ch
slug: learn-frontend-web-development-in-12-days-advanced-css
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1685618396925/a58c7f8d-28b5-4d7b-9410-7d9056190720.webp
tags: tutorial, css, web-development, beginners, frontend-development

---

Hello and welcome! 🤩🤩🤩

Today is our second day talking about CSS. We had a pretty good landing last week and understood some basic and core CSS principles and syntax.

In today's lesson, we will dive deeper into some cool things we can do with CSS.

CSS is all about styling, and with styling, there is so much you can do. This article does not cover all the possibilities available with CSS, but it will give you a great guide to figuring things out independently.

## CSS Layout

***Stacking context*** *is a three-dimensional conceptualization of HTML elements along an imaginary z-axis relative to the user, who is assumed to be facing the viewport or the webpage. HTML elements occupy this space in priority order based on their attributes.*

### CSS Position property

The CSS `position` property specifies the type of positioning method used for an element. There are five different position values: `static`, `relative`, `fixed`, `absolute,` and `sticky.`

**Static**: HTML elements are positioned static by default. `static` *position elements are not affected by the* `top`*,* `bottom`*,* `left`*, and* `right` *CSS properties.* An element with `position: static;` is not positioned in any special way; it is always positioned according to the normal flow of the page.

**Relative**: An element with `position: relative;` is positioned relative to its normal position. Setting the `top`, `right`, `bottom`, and `left` properties of a relatively-positioned element will cause it to be adjusted away from its normal position.

<iframe height="300" style="width:100%" src="https://codepen.io/dumebii/embed/WNaqYbY?default-tab=html%2Cresult">
  See the Pen <a href="https://codepen.io/dumebii/pen/WNaqYbY">
  Untitled</a> by Dumebi Okolo (<a href="https://codepen.io/dumebii">@dumebii</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

Notice in the codepen above how we have been able to move the position of the green container.

**Fixed**: An element with `position: fixed;` is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled. The top, right, bottom, and left properties are used to position the element. *A fixed element does not leave a gap in the page where it would normally have been located.*

<iframe height="265" style="width:100%" src="https://codepen.io/dumebii/embed/Rwezqaj?default-tab=html%2Cresult">
  See the Pen <a href="https://codepen.io/dumebii/pen/Rwezqaj">
  Untitled</a> by Dumebi Okolo (<a href="https://codepen.io/dumebii">@dumebii</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

In the example above, we notice that the `h2` element is shown on our screen even when we scroll down past it.

**Absolute**: An element with `position: absolute;` is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed). However, if an `absolute` positioned element has no positioned ancestors, it uses the document body, and moves along with page scrolling.

***Note:*** `absolute` *positioned elements are removed from the normal flow and can overlap elements.*

<iframe height="218" style="width:100%" src="https://codepen.io/dumebii/embed/vYVqQrj?default-tab=html%2Cresult">
  See the Pen <a href="https://codepen.io/dumebii/pen/vYVqQrj">
  Untitled</a> by Dumebi Okolo (<a href="https://codepen.io/dumebii">@dumebii</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

In the example above, we see that the second container's position is being modified based on the position of the element preceding it.

**Sticky**: An element with `position: sticky;` is positioned based on the user's scroll position. A sticky element toggles between `relative` and `fixed`, depending on the scroll position. It is positioned relative until a given offset position is met in the viewport - then it "sticks" in place (like `position:fixed`).

***Note:*** *Internet Explorer does not support sticky positioning. Safari requires a* `-webkit-` *prefix (see example below). You must also specify at least one of* `top`*,* `right`*,* `bottom` *or* `left` *for sticky positioning to work.*

<iframe height="188" style="width:100%" src="https://codepen.io/dumebii/embed/Rwezqde?default-tab=html%2Cresult">
  See the Pen <a href="https://codepen.io/dumebii/pen/Rwezqde">
  Untitled</a> by Dumebi Okolo (<a href="https://codepen.io/dumebii">@dumebii</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

In the example above, we see that the green container has maintained a fixed position, regardless of our scrolling through the page.

### CSS Flex box

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1685615223207/2f8b989e-73cf-4805-a6f8-59469ac625ee.png align="center")

Flexbox is a powerful layout model that simplifies the creation of flexible and responsive layouts. It allows you to align and distribute elements within a container, making it easier to build complex designs. With properties like `flex-direction`, `justify-content`, and `align-items`, you can achieve versatile and dynamic layouts.

<iframe height="300" style="width:100%" src="https://codepen.io/dumebii/embed/VwEJqLG?default-tab=html%2Cresult">
  See the Pen <a href="https://codepen.io/dumebii/pen/VwEJqLG">
  Untitled</a> by Dumebi Okolo (<a href="https://codepen.io/dumebii">@dumebii</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

We can see how, in the example above, we were able to position our paragraphs next to each other, with ample space between them with just two lines of CSS. This is the power of the CSS flexbox. There is a lot more that can be done with the CSS flexbox.

### CSS Grid

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1685616078948/db1f1298-b907-4971-9fd0-229c4ca63d21.png align="center")

CSS Grid provides a two-dimensional layout system that enables precise control over rows and columns. It allows you to create complex grid structures and define the placement and sizing of elements. With features like grid templates, grid areas, and grid alignment, you can design sophisticated and visually appealing layouts.

## Media Queries

Responsive web design is crucial in today's mobile-driven world. Media queries allow you to create responsive layouts that adapt to different screen sizes. By defining different CSS rules based on media query breakpoints, you can adjust the design, font sizes, and layouts to provide optimal user experiences across various devices. In my article about whether a developer should go with [Mobile first or Desktop first](https://dumebi.hashnode.dev/mobile-first-or-desktop-first-development) website design, I talked a bit more about what responsive design is.

```css
/* Example of a media query for responsive design */
@media screen and (max-width: 768px) {
  /* CSS rules for smaller screens */
  /* Adjust the layout, font sizes, etc. */
}
```

In the code block above, there is a sample syntax for writing a media query for a device whose maximum width is 768px. After defining your media breakpoint, you write your CSS code in between the curly braces as you would normal CSS. The properties you specify here will only take effect when the device width is at the specified value.

## Transitions and Animations

With CSS, there are lots of cool and flashy stylings we can add to our website to make it more visually appealing. A cool way we can do this is by using CSS transitions and animations. You can go the extra mile by learning how to personally create these animations and transitions and even coming up with a few of your own. However, there are these packages called **CSS transition libraries,** which are other people's CSS transition or animation effects already written and ready for use. Here are a few:

* [Animista](http://animista.net/)
    
* [Animate.css](https://daneden.github.io/animate.css/)
    
* [Tachyons-animate](https://github.com/anater/tachyons-animate)
    
* [Infinite](http://tilomitra.github.io/infinite/)
    

There are a lot more transition and animation libraries available. You can even create your own! 😏😏

## CSS Blend Modes

CSS blend modes offer creative possibilities by controlling how elements blend with the background or other elements. By applying blend modes to elements, you can create stunning overlays, image effects, and blending compositions. Some common blend mode values include `multiply`, `screen`, `overlay`, and `soft-light`.

<iframe height="272" style="width:100%" src="https://codepen.io/dumebii/embed/QWZXzov?default-tab=html%2Cresult">
  See the Pen <a href="https://codepen.io/dumebii/pen/QWZXzov">
  Untitled</a> by Dumebi Okolo (<a href="https://codepen.io/dumebii">@dumebii</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

In the codepen above, we can see the effect the different blend modes are having on the containers. Each container has a background color of red on a black body.

## CSS Variables

CSS variables, also known as custom properties, introduce the concept of reusable values throughout your CSS codebase. By defining variables, you can easily change and update common values across your stylesheets, providing consistency and flexibility. CSS variables also allow you to create dynamic themes and styles by modifying variable values with JavaScript.

```css
/* Example of defining and using a CSS variable */
:root {
  --primary-color: #007bff;
}

.my-element {
  color: var(--primary-color);
}
```

Wooosh! This was a long one, but I think it was totally worth it! I think we have done justice to foundational CSS and given enough insight into the things you need to know to get grinding! 🤩🤩🤩

## References

[Transitions and Animations](https://css-tricks.com/css-animation-libraries/)

[CSS Positions](https://www.w3schools.com/css/css_positioning.asp)

[Flex box image](https://marina-ferreira.github.io/tutorials/css/flexbox/)

[HTML stacking](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_positioned_layout/Understanding_z-index/Stacking_context)

[CSS Grid image](https://learn.microsoft.com/en-us/microsoft-edge/devtools-guide-chromium/css/grid)

[Cover Image](https://www.geeksforgeeks.org/css/)

[My trusty chatGPT 🥳🥳](http://chat.openai.com)