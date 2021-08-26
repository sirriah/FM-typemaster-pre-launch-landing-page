# Frontend Mentor - Typemaster pre-launch landing page solution

This is my solution to the [Typemaster pre-launch landing page challenge on Frontend Mentor](). 
I love Frontend Mentor ❤️‍🔥 and I am happy that I can be a PRO.

## Table of contents

- [Frontend Mentor - Typemaster pre-launch landing page solution](#frontend-mentor---typemaster-pre-launch-landing-page-solution)
  - [Table of contents](#table-of-contents)
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



## Overview

### The challenge

Users should be able to display the web page. No interaction is there - only hover effect on buttons.

-

### Screenshot

![](./preview.jpg)


### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- SASS, BEM
- Flexbox
- CSS Grid
- Mobile-first workflow



### What I learned

I am still beginner in creating my own mixins or extends. But I try to use it in this project. 
I used the extend for the "details" part with icons. I defined the style of one item and then I extend it with icon image.



To see how you can add code snippets, see below:

```html
<section class="details container">
        <h2 class="sr-only">Details list</h2>
        <ul>
          <li class="details__icon--compatible">
            <h3>Highly compatible</h3>
            <p>
              Easy to use and works well with all major computer brands, gaming
              consoles and mobile devices. Plug & play, no installation or
              driver needed.
            </p>
          </li>
          <li class="details__icon--bluetooth">
            <h3>Wireless with bluetooth</h3>
            <p>
              Powerful 2.4G RF technology allows you to connect the cordless
              keyboard from up to 30ft away. Simply plug the unifying receiver
              into your computer.
            </p>
          </li>
          <li class="details__icon--battery">
            <h3>High capacity battery</h3>
            <p>
              Equipped with a long-lasting built-in battery, you’ll never have
              to spend a dime on replaceable ones. Enjoy 40 hours of usage time
              between charges.
            </p>
          </li>
          <li class="details__icon--light">
            <h3>RGB backlit modes</h3>
            <p>
              Choose from 4 backlight brightness levels and adjustable breathing
              speed. Each key glows intensely in the dark and helps you type in
              low light conditions.
            </p>
          </li>
        </ul>
      </section>
```

```css
&__icon--compatible:before {
    content: "";
    width: 4.0625rem;
    height: 4.0625rem;
    display: inline-block;
    border-radius: 1rem;
    margin-bottom: 3rem;
    background-image: url("./../assets/shared/icon-compatible.svg");
    background-repeat: no-repeat;
    background-position: center center;
    background-color: abstracts.$primary-500;
  }

  &__icon--bluetooth:before {
    @extend .details__icon--compatible;
    background-image: url("./../assets/shared/icon-bluetooth.svg");
  }

  &__icon--battery:before {
    @extend .details__icon--compatible;
    background-image: url("./../assets/shared/icon-battery.svg");
  }

  &__icon--light:before {
    @extend .details__icon--compatible;
    background-image: url("./../assets/shared/icon-light.svg");
  }
```



### Continued development

I made this project after the long time and I need to remind some things. For the next challenges I would like to use some advanced techniques of SASS. 

### Useful resources

- [A complete guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/) - This always helps me with setting of CSS Grid.
- [A complete guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - And same for this with Flexbox 😀



## Author

- Frontend Mentor - [@sirriah](https://www.frontendmentor.io/profile/sirriah)

