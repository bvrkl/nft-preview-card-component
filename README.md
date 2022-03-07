# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

[Solution](./images/nftProjectScreenshot.jpg)

### Links

- Live Site URL: [Live Site URL](https://nft-preview-card-component-main-qze6r4op2-bvrkl.vercel.app/)

## My process

-It is only a simple task so there is not much detail that I feel I need to go into.

-I first made my HTML file with all the appropriate images, text, and class names to use later, so the only thing I had left to do would be to style it all.

-I worked from the biggest to the smallest when styling, so first I sized and coloured the outermost div, then when i was happy I moved onto it's children.

-The only hiccup I had was after I had finished the styling aside from adding the hover reactivity. Naturally, the preview card responded to resolution changes because I used flex box to center and manipulate most of the contents spacing etc, so worrying about the transition from my small resolution (mobile) to a larger monitor size was not necessary.
-I only added a single media query for a mobile size, to deal with the empty space that would appear above the card

-To add the hover interactivity, i simply used the :hover method in css, to avoid any javascript or extra classes being added.

-I was unsure on how- upon hovering over the image- to get the extra icon and cyan overlay to appear. After being unable to find a way to "create a new div", I simply lowered the opacity of the image and changed the background to my ideal overlay. While it may not be the best way to go about this, I felt in the environment of this exercise, as it was only a small task, it would not be necessary to worry about it too much.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flex box
- CSS Grid
- Mobile-first workflow

### What I learned

This exercise really helped reinforce some simple, healthy practices, and also techniques which I felt are useful in the long run to get most comfortable with.

I had never used the :hover functionality before, so getting to grips with how to use it and coming up for a quick fix for my problem was definitely a notable accomplishment in this exercise.

```css
.image img:hover {
  cursor: pointer;
  opacity: 20%;
}

.image:hover {
  background-image: url("./images/icon-view.svg");
  background-repeat: no-repeat;
  background-color: hsl(178, 100%, 50%);
  background-position: center;
}
```

A quick revisit to the strange media query syntax also was refreshing

```css
@media only screen and (max-width: 550px) {
  .container {
    margin-top: 75px;
  }
}
```

As for HTML, I have previously learned the hard way how much easier using as many divs to group content into sections as possible makes the styling process. It would be too much to paste here but it is clearly demonstrated in my HTML file, and the heavy use of classes etc. I found gave me easy control over every element on the page.

### Continued development

There is certainly room to improve on my CSS skills, and perhaps learning new ways of doing the same things but better, as I find that perhaps my css file has too many declaration blocks that only style one small part of the site. Therefore, I could improve making everything more concise and readable for the next person reading it.

Analysing my own work would also be something I need much more practice on as that is something I do not often do.

## Author

- Frontend Mentor - [@bvrkl](https://www.frontendmentor.io/profile/bvrkl)
