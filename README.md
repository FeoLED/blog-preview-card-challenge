# Frontend Mentor - Blog preview card solution

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshots](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)


## Overview

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page

### Screenshots

Laptop browser preview:

![](browser-preview.png)

Phone preview: 

![](phone-preview.png)

### Links

- Solution URL: ![GitHub repository](https://github.com/FeoLED/blog-preview-card-challenge)

- Live Site URL: ![Live Site](https://feoled.github.io/blog-preview-card-challenge/)


## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

   In the developing of this, I mostly reinforced things that I learned. The road consisted mostly on figuring out how to proceed and bumping into CSS related trouble.
    For starters, I tend to apply borders on important containers to test boundaries and the space they occupy (and if there's no container, I create it to test)
    At the beginning, I focused on the head elements, like meta tags, removing the style tag, and moving the styles to a external CSS file.
    As I proceed to add colors, I had to juggle with how flexbox affected the display of inner elements. So what I did? More divs.
    I faced a design problem attempting to align the card content to the left. Using flexbox and "justify-items:left" didn't work. Past experiences with "margin"* inspired me to try "margin-right:auto", solving the problem.
    *This past experience is related with keeping the footer at the bottom of the page. It includes adding a display flex to the parent and then giving margin-top:auto to footer. If that worked for the footer, it must work for the elements in the card*
    Near the end I got a particularly nasty problem with the card elements: While reducing the browser's height(a foolish thing to focus on but I was paranoid) the bottom elements broke out of the parent element. It gave a feeling that they were "sliding away". Further research told me it was an overflow problem.
    Among the solutions presented, there was manipulating the "overflow" property. After trying different options, I default for "scroll":

```
.card{
  overflow:scroll;
}
```
With this, when the viewport's height changes, the card will show a scrollbar, keeping the elements withing their righful boundaries. I wasn't happy with this but it was the least ugly solution at the time.


### Continued development

I'm not quite familiar with overflow control methods. Knowing that future projects would be more complex, I want to learn more about content management. 


## Author

- Website - ![GitHub profile](https://github.com/FeoLED)
- Frontend Mentor - ![@FeoLED](https://www.frontendmentor.io/profile/FeoLED)
