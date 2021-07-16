# Frontend Mentor - Huddle landing page with single introductory section solution

This is a solution to the [Huddle landing page with single introductory section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/huddle-landing-page-with-a-single-introductory-section-B_2Wvxgi0). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![./images/Web%20capture_29-6-2021_74141_txmack713.github.io]

### Links

- Solution URL: [GitHub/TXMack713](https://github.com/TXMack713/huddle-landing-page)
- Live Site URL: [GitHub Pages] (https://txmack713.github.io/huddle-landing-page/)

## My process

I started with the mobile layout first and then after I was satisfied with the mobile layout, I proceeded to create the desktop layout. After observing how disproportionate the size of the `.landing` and `#layouts` sections were, I created a second desktop layout for smaller screens that incorporated a smaller heading size for better proportions between the `#layouts` image and the `.landing` paragraph.

I checked other learners' code on frontendmentor.io to see how they were solving the issue of sizing and positioning the desktop background image to better match the desktop's design preview. I began by working on adjusting only the size of the background using the various keywords and then began working on moving the `#layouts` and `.landing` sections up and down within the grid, but after researching background positioning articles on css-tricks and W3Schools, I changed the background's psotionining from `center` `center` to `bottom` `center` and the size from `cover` to `auto`.

Finally, I changed the mobile layout's `icon` positioning from flexbox to grid for greater control over the spacing.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid
- Mobile-first workflow

### What I learned

I chose to use CSS Grid to have better control over the placement of the sections to get them exactly where I wanted.

I paid careful attention to the spacing of between the different sections by examining closely the space between the sections on my rendered page versus the spacing shown on the desktop and mobile previews.

I learned that using percentages rendered the layout of the page in line with my expectations better than using vw and vh for units. When using vw and vh, the elements were jumbled together and would overlap no matter how much I increased or descreased the size of the gaps and tracks within the body and section elements. By switching to percentages, the page rendered as expected and allowed me to fine tune the layout, moving and tweaking item placements as necessary to better match the design.

I experimented with the box-shadow property and enlarged the blur-radius to get a more pronounced visual effect in the desktop layout where the design was spread out over multiple columns versus the single column in the mobile layout.

```css
body {
    display: grid;
    grid-template-rows: 10% 10% repeat(5, 12.5%) 17.5%;
    grid-template-columns: repeat(11, 1fr);
    grid-column-gap: 30px;
    grid-row-gap: 10px;
    padding: 2rem 0;
    max-inline-size: 1440px;
  }

  .calculator {
  border-top: 3px solid hsl(212, 86%, 64%);
  box-shadow: 0 5px 5px hsl(229, 6%, 66%);
}

.calculator {
    border-top: 3px solid hsl(212, 86%, 64%);
    box-shadow: 0 5px 10px hsl(229, 6%, 66%);
  }
```

### Continued development

- I'm continuing to learn CSS layout, particularly CSS Grid as I find that I have greater control over and confidence in the placement of items in my layouts.

### Useful resources
- The MDN Web Docs (https://developer.mozilla.org/en-US/) proved to be invaluable for quick lookups regarding the different values for certain properties, specifically with centering the content as expected within the containers.

## Author

- Website - [Anthony Mack](https://txmack713.github.io/huddle-landing-page/)
- Frontend Mentor - [@TXMack713](https://www.frontendmentor.io/profile/txmack713)

### Acknowledgements
