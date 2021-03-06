# Frontend Mentor - Launch countdown timer solution

This is a solution to the [Launch countdown timer challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/launch-countdown-timer-N0XkGfyz-). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

## Overview

### The challenge

Users should be able to:

- See hover states for all interactive elements on the page
- See a live countdown timer that ticks down every second (start the count at 14 days)
- **Bonus**: When a number changes, make the card flip from the middle

### Screenshot

![here](./images/screenshot/Screenshot%202022-05-25%20at%205.49.46%20PM.png)


### Links

- Live Site URL: [Here](https://rishi1011.github.io/launch-countdown-timer/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

This project was really helpful in learning both javascript and CSS.
 - In javascript, I learned new things in manipulation of dates.
 - Also learned about data attributes that are used to select and manipulate tags from javascript.
 - In CSS, learning about flip animation made me realise animations in deeper.

 For the flip-animation, I added divs on top containing the same content. Then I used `transform: rotateX(90deg)` on the cards making it happen in 0.5s. Note that there are two divs top-flip and bottom-flip, bottom-flip happens halfway after top-flip animation ends. Used `transformation-origin: top` on bottom-flip.

 ```
    @keyframes flip-top {
        to {
            transform: rotateX(90deg);
        }
    }

    @keyframes flip-bottom {
        to {
            transform: rotateX(0deg);
        }
    }
 ```

 **The top-flip transforms from 0 to 90deg, whereas bottom-flip transforms from 90deg to 0.**

### Continued development

Areas which I'd like to improve upon:
- Inset rounded corners in the card div.
- Give a perspective to the flip-animation.

### Useful resources

- [draft-countdown codepen](https://codepen.io/doriancami/full/jEJvaV) - I really liked this pattern and will use it going forward.
- [draft-countdown tutorial](https://www.youtube.com/watch?v=p_6IuhmBsfc) - This is an amazing video which helped me finally understand flip animation. I'd recommend it to anyone who needs clarify in implementing it.
- [Change color in SVG] (https://stackoverflow.com/questions/22252472/how-to-change-the-color-of-an-svg-element) Colors can be changed in svg images through filter, a color can be transformed to filter properties through this link. Found this really helpful!

## Author

- Frontend Mentor - [@rishi1011](https://www.frontendmentor.io/profile/rishi1011)
- Twitter - [@rishikrishna_r](https://www.twitter.com/rishikrishna_r)

## Acknowledgments

I would like to give credit to [Kyle from WebDevSimplified](https://www.youtube.com/c/WebDevSimplified) from whom I learned the most.



