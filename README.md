# Frontend Mentor - News homepage solution

This is a solution to the [News homepage challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/news-homepage-H6SWTa1MFl). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page

### Screenshot

![](./design/screenshots/Screen%20Shot%202023-08-02%20at%2002.48.14.png)
![](./design/screenshots/Screen%20Shot%202023-08-02%20at%2002.48.37.png)





### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Desktop-first workflow
- Jscript
- Media Querry



### What I learned

I learnt how to properly assign data vissibility and aria expanded

```html
<button class="mobile-nav-toggle" aria-controls="nav"  aria-expanded="false">
      <span class="sr-only " style="display: none;" >Menu</span>
    </button>
```
```css
.mobile-nav-toggle[aria-expanded = "true"]{
    background-image: url(/news-homepage-main/assets/images/icon-menu-close.svg);


.nav[ data-visible ="true"]{
  transform: translateX(0%);
}
```
```js
navToggle.addEventListener('click', () => {
    const visibillity = primaryNav.getAttribute('data-visible');
    
    if (visibillity === "false") {
        primaryNav.setAttribute('data-visible', true);
        navToggle.setAttribute('aria-expanded', true);
    }else if(visibillity === "true"){
        primaryNav.setAttribute('data-visible', false);
        navToggle.setAttribute('aria-expanded', false);
    };
  
});

```


### Continued development
I would like to work more on the usagge of the above method as it makes the whole cod eneat and structured


### Useful resources

- [Kevin Powell](https://www.youtube.com/@KevinPowell) - This helped me to undersstand the use of aria expanded and data vissibility

## Author


- Frontend Mentor - [@lastiroko](https://www.frontendmentor.io/profile/lastiroko)




## Acknowledgments

Thank myself and my Maker.

