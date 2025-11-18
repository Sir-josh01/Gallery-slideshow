# Rotating Image Gallery
This project is a classic UI carousel (or slider) designed to showcase multiple images in a compact, rotating space. Built purely with Vanilla JavaScript, HTML, and CSS, it features both automatic rotation and manual navigation controls. It serves as a strong demonstration of dynamic DOM manipulation and efficient, framework-free UI development.

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

The Image Carousel is a fundamental user interface component designed to efficiently showcase a collection of images or content in a compact, cyclical manner. Developed entirely using vanilla JavaScript, HTML, and CSS, this project demonstrates mastery of dynamic content manipulation and modern front-end interaction..

### The challenge

-Getting the images to rotate after a specific stimulated time.
-Making the image of same size and rotate accordingly

### Screenshot

![](./Screenshots/Screenshot%20(200).png)
![](./Screenshots/Screenshot%20(204).png)
![](./Screenshots/Screenshot%20(205).png)

### Links

- Solution URL: [@GitHub]( https://github.com/Sir-josh01/rotating-image-gallery.git)
- Live Site URL: [@](https://sir-josh01.github.io/)

## My process
- Structure with HTML, 
- Designs and color by CSS 
- Handles the functionality and animation   with vanilla Javascript only.

### Built with
- Semantic HTML5 markup
- CSS custom properties
- Javascript for interaction

### What I learned

```html
<h1>
  <!-- Proud of this syntax -->
  <div class="date-box">
    <label for="days">DAY</label>
    <input type="text" placeholder="DD" class="day-input" required />
    <div class="error-msg">Must be a valid day</div>
  </div>
</h1>
```

```css
.image-container {
  width: 200px;
  height: 200px;
  transform-style: preserve-3d;
  transform: perspective(1000px) rotateY(0deg);
  transition: transform .7s;
}

.image-container span {
  position: absolute;
  left: 0;
  top: 0;
  transform: rotateY(calc(var(--i)*45deg)) translateZ(400px);
  width: 100%;
}
```

```js
let x = 0;
let timer;
prevBtn.addEventListener('click', () => {
  x += 45;
  clearTimeout(timer)
  updateGallery();
})

nextBtn.addEventListener('click', () => {
  x -= 45;
  clearTimeout(timer)
  updateGallery();
})};
```

### Continued development

-To add an API and integrate the application to change multiple images
-Add a button that makes the rotation stop and another that increases the speed  

### Useful resources

- [Example resource 1](https://www.google.com) - Acquired some resources from stackoverflow.
- [Example resource 2](https://www.w3school/CSS-animation.com) - An amazing site which helped with giving understanding alittle deeper about the concept of animation.


## Author

- Website - [@sir_josh01](https://www.your-site.com)
- Frontend Mentor - [@sir_josh01](https://www.frontendmentor.io/profile/sir_josh01)
- Twitter - [@sir_josh01](https://www.twitter.com/Sir_josh01)
- LinkedIn - [@sir_josh01](https://www.linkedin.com/in/sir-josh01)

