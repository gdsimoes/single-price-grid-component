# Frontend Mentor - Single price grid component solution

This is a solution to the [Single price grid component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/single-price-grid-component-5ce41129d0ff452fec5abbbc). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

-   [Overview](#overview)
    -   [The challenge](#the-challenge)
    -   [Screenshots](#screenshots)
    -   [Links](#links)
-   [My process](#my-process)
    -   [Built with](#built-with)
    -   [What I learned](#what-i-learned)
    -   [Continued development](#continued-development)
    -   [Useful resources](#useful-resources)
-   [Author](#author)

## Overview

### The challenge

Users should be able to:

-   View the optimal layout for the component depending on their device's screen size
-   See a hover state on desktop for the Sign Up call-to-action

### Screenshots

-   Desktop

<img src="./screenDesktop.gif" alt="GIF of the website on desktop">

-   Mobile

<img src="./screenMobile.png" alt="GIF of the website on desktop" width="15%">

### Links

-   Solution URL: <https://github.com/gdsimoes/single-price-grid-component>
-   Live Site URL: <https://gdsimoes.github.io/single-price-grid-component>

## My process

### Built with

-   Semantic HTML5 markup
-   Flexbox
-   CSS Grid
-   Mobile-first workflow
-   [Sass](https://sass-lang.com/) - CSS extension language

### What I learned

In this project, I tried learning two new technologies at once: CSS Grids and Sass. I was able to pull this off, and I am very proud of the results. Since I wanted to use at least one nontrivial Sass feature, I used mixins for my media queries like this:

```scss
@mixin desktop {
    @media (min-width: 1440px) {
        @content;
    }
}
// ...

@include desktop {
    font-size: 2.4vw;
    margin-right: 0.4vw;
}
```

I also wanted to create this website using `grid-template-areas` because I feel like this is the most straightforward way of describing a layout. The result is relatively easy to understand:

```scss
main {
    // ...
    grid-template-areas:
        "pitch pitch"
        "subscription details";
}
```

### Continued development

I realize I only scratched the surface of what can be achieved with CSS Grid, and I am looking forward to improving my skills on the following projects.

### Useful resources

-   [A Complete Guide to Grid | CSS-Tricks](https://css-tricks.com/snippets/css/complete-guide-grid/) - Once again, CSS-Tricks saves the day. Like their famous Flexbox guide, this page contains all the essential information concisely and clearly.
-   [Build a Classic Layout FAST in CSS Grid | MDN](https://www.youtube.com/watch?v=KOvGeFUHAC0) - This short video shows how to create a simple layout using CSS Grid. Sometimes seeing a more experienced programmer in action can be very elucidating in learning how to do something.

## Author

-   Website - <https://gdsimoes.com>
-   Frontend Mentor - [@gdsimoes](https://www.frontendmentor.io/profile/gdsimoes)
-   LinkedIn - [Guilherme Dias Simoes](https://www.linkedin.com/in/gdsimoes)
