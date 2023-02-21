# Boolean Academy - Responsive Website Logo

This is a solution to the Esercizio 11 - Boolean - 20 February 2023.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
  - [Design Provided](#design-provided)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)


## Overview

### The challenge

- Build out the project to the designs provided with three sizes: Mobile/Tablet/Desktop

### Links

- Solution URL: [https://github.com/filecc/htmlcss-responsive-layout](https://github.com/filecc/htmlcss-responsive-layout)
- Live Site URL: [https://filecc.github.io/htmlcss-responsive-layout/](https://filecc.github.io/htmlcss-responsive-layout/)

### Design Provided

## Desktop Design
![Desktop](./design/Responsive-Layout-Desktop.png)

## Tablet Design
![Tablet](./design/Responsive-Layout-Tablet.png)

## Mobile Design
![Mobile](./design/Responsive-Layout-Mobile.png)


## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

We are required not to use any framework, so I rewrite all the classes I used after directly in the project in 'utilities.css' file.


```css
/* positionts */
.fixed{
    position: fixed;
}
.relative{
    position: relative;
}
.absolute{
    position: absolute;
}

/* borde radius */
.rounded-sm{
    border-radius: 10px;
}
.rounded-md{
    border-radius: 20px;
}
.rounded-lg{
    border-radius: 40px;
}
.rounded-full{
    border-radius: 100%;
}
```
```html
 <div class="lg-p-3 lg-w40">
                    <div>
                        <img class="pt-3 mx-auto" aria-hidden="true" src="./img/planning1.png" alt="planning">
                    </div>
                    <div>
                        <h2 class="text-white text-lg mt-6 sm-text-xl lg-text-md">Strategic Planning</h2>
                        <p class="text-white pt-2 text-sm">Lorem ipsum dolor sit, amet consectetur adipisicing elit.
                            Distinctio
                            quos assumenda voluptas non fugiat in culpa, numquam atque nobis expedita aperiam nam unde
                            sapiente nisi. Excepturi ad porro non, beatae expedita illo error atque, provident commodi a
                            repellat ab ipsum!</p>
                    </div>
                </div>
```

For the hamburger manu, that is working, I started from an input checkbox that act like a click receiver.

```html
<div id="hamburger">
                <input class="" type="checkbox">
                <i id="openBtn" class="fa-solid fa-bars text-md"></i>
                <i id="closeBtn" class="fa-solid fa-xmark text-md"></i>
                <div id="menu" class="hidden relative w-full flex flex-col justify-center align-center">
                    <div class="mb-3">
                        <img aria-hidden="true" src="./img/logo.png" alt="logo">
                    </div>
                    <ul class="flex flex-col justify-center align-center w-full">
                        <li> <a href="#planning">Planning</a></li>
                        <li><a href="#testimonials">Testimonials</a></li>
                        <li><a href="#features">Features</a></li>
                        <li><a href="#aboutus">About Us</a></li>
                    </ul>
                </div>
            </div>
````

and I styled it with css using it to hide/show the menu in Tablet/Mobile view.
