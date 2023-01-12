# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### Screenshot

![Page Screenshot](/images/qr-component.jpg)

### Links

- Solution URL: [Frontend Mentor](https://www.frontendmentor.io/solutions/qr-code-component-HJ4Cv1suXS)
- Live Site URL: [Github Pages](https://kyr27.github.io/qr-code-component-main/)

## My process

### Built with

- Semantic HTML5 markup
- Flexbox
- [CSS Reset](https://piccalil.li/blog/a-modern-css-reset/)
- CSS custom properties
- Mobile-first workflow
- [Google Fonts](https://fonts.google.com/specimen/Outfit)

### What I learned

I've learned how to add fonts from google fonts, learned how to center a div, learned how to use CSS variables, learned about media queries, learned about image filters, learned to avoid pixels except when dealing with small sizes, as they do not scale responsively, you should instead use rem or em units, the difference between rem and em being that rem scales with default font size, while em scales with parent size. learned about CSS resets and added one(however i might use html5boilerplate next time instead. I've thought about using it here aswell but it was too large and complex for this small project)

I'd also like to point out that figuring out how to center the div took way longer than it should have, i looked at many videos and examples on how to center it using flexbox but not 1 of them mentioned that you must first set the height of the div container. This is something that is extremely easy to overlook when you don't have any experience in web development, especially considering you do not have to do this for the width, only the height.

```html
<div class="card-container">
  <div class="card">
    <div class="card-image">
      <img src="images/image-qr-code.png" alt="QR Code Image" />
    </div>
    <div class="card-header">
      Improve your front-end skills by building projects
    </div>
    <div class="card-content">
      Scan the QR code to visit Frontend Mentor and take your coding skills to
      the next level
    </div>
  </div>
</div>
```

```css
/* Responsively centers the card using Flexbox */
.card-container {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
}
/* Automatically switches from light theme to dark theme if the user has their browser scheme set to dark. This also uses filters to hue shift the image into the green colors for lessening the eye strain when looking at the image*/
@media (prefers-color-scheme: dark) {
  :root {
    --foreground-color: var(--foreground-color-dark);
    --background-color: var(--background-color-dark);

    --header-color: var(--header-color-dark);
    --paragraph-color: var(--paragraph-color-dark);
  }

  img {
    filter: brightness(0.8);
    -webkit-filter: brightness(0.8);

    filter: hue-rotate(280deg);
    -webkit-filter: hue-rotate(280deg);
  }
}
```

### Continued development

I'd like to learn more about CSS Grid, Flexbox, transitions, aria, DOM Manipulation, Electron, proper website layout and backend web development. Once im confident in these i will learn Sass/scss and other frameworks and extensions like React, Redux and perhaps Post CSS.

### Useful resources

[Kevin Powell](https://www.youtube.com/@KevinPowell)
for his excellent YouTube tutorials, i can not describe how much he has helped me with learning web development.

[Modern CSS](moderncss.dev)
Has a lot of useful resources there, i've learned how to always position the footer to the bottom of the screen thanks to her.

[Solo Learn](sololearn.com)
Helped me get started with web development. At this point in time i've yet to finish their basic course on web development.

[Piccalil](https://piccalil.li)
For the amazing CSS Reset that i've used in this project.
The site has a ton more useful resources that i've yet to learn.

[Free Code Camp](https://www.freecodecamp.org)
Started a course there on Responsive Web Development recently and learned a few things, i will be visiting this site quite a bit going forward, as it has everything i want to learn.

[Frontend Mentor](https://www.frontendmentor.io)
For the designs and guidelines, an amazing resource that lets you focus on the development aspect, instead of trying to both learn designing and web development at the same time.

## Author

- Frontend Mentor - [Kyr27](https://www.frontendmentor.io/profile/Kyr27)
