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
- [Author](#author)

================================================================================================

## Overview

### Screenshot

![the solution screenshot](/screenshot.jpg)

================================================================================================

## My process

I am a French beginner developer, I started learning HTML and CSS a few weeks ago. 
This is my second project on Frontend Mentor, and this time I tried to do it without using photoshop to take the dimensions.   
I made my html without any problem, even if I changed the structure of it so many times. 

The biggest problem I had with this project was the image, at first I had put it directly in the html 
but when I had to do the hover effect, I had some problems. 
In the end I just put an empty div and add the image directly with the css. 
Unfortunately, I didn't manage to make exactly the same hover effect as on the design, 
I don't know how to change the background color of the svg, moreover, I had problems to manage to center it. 
In the end, to center it I had to put it in "cover" because with the small size, I could not put it in the center. 

### Built with

- Semantic HTML5 markup
- CSS basic properties

================================================================================================

### What I learned

I learned that you can do a lot more than I thought with the '::before, ::after' properties, 
here is an example, even if I didn't manage to get the result I wanted:
``` css
.image {
    position: relative;
    width: 335px;
    height: 335px;
    background: url(images/image-equilibrium.jpg) center center / cover no-repeat;
    border-radius: 10px;
    box-shadow: 1px 4px 10px 1px rgba(0, 0, 0, 0.3);

}
.image::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    height: 335px;
    width: 335px;
    transition: all 0.3s;
    opacity: 0;
    background: url(images/icon-view.svg) no-repeat;
    background-size: cover;
    cursor: pointer;
}
.image:hover:before {
    opacity: 0.5;
}
```
================================================================================================

### Continued development
I would like to add features that would use javascript like counting down the days left after each day. But, as I haven't started learning JS yet, it will wait. 

================================================================================================

## Author

- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/sid-shinseo)
