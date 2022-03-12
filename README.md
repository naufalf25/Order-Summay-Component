# Frontend Mentor - Order summary card solution

This is a solution to the [Order summary card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/order-summary-component-QlPmajDUj). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- See hover states for interactive elements

### Screenshot

![./design/myDesign.png]

### Links

- Solution URL: [https://github.com/naufalf25/Order-Summay-Component]
- Live Site URL: [https://naufalf25.github.io/Order-Summay-Component/]

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid

### What I learned

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

To see how you can add code snippets, see below:

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <link rel="icon" type="image/png" sizes="32x32" href="./images/favicon-32x32.png">
        <title>Frontend Mentor | Order summary card</title>
        <link rel="stylesheet" href="style.css">
    </head>
    <body>
        <div class="container">
            <div class="card">
                <img src="images/illustration-hero.svg" alt="hero">
                <div class="content">
                    <h2>Order Summary</h2>
                    <p>You can now listen to millions of songs, audiobooks, and podcasts on any 
                    device anywhere you like!</p>
                    <div class="annual">
                        <img src="images/icon-music.svg" alt="" aria-label="hidden">
                        <div class="price">
                            <p class="price-head">Annual Plan</p>
                            <p class="price-body">$59.99/year</p>
                        </div>
                        <a href="#"><p>Change</p></a>
                    </div>
                    <div class="order-btn">
                        <a href="#">Proceed to Payment</a>
                    </div>
                    <div class="cancel-btn">
                        <a href="#">Cancel Order</a>
                    </div>
                </div>
            </div>
        </div>
    </body>
</html>
```
```css
*, *::before, *::after {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

:root {
    --color-paleblue: hsl(225, 100%, 94%);
    --color-brightblue: hsl(245, 75%, 52%);
    --color-verypaleblue: hsl(225, 100%, 98%);
    --color-desaturatedblue: hsl(224, 23%, 55%);
    --color-darkblue: hsl(223, 47%, 23%);
}

@import url('https://fonts.googleapis.com/css2?family=Red+Hat+Display:ital,wght@0,500;0,700;0,900;1,500;1,700;1,900&display=swap');

body {
    font-family: 'Red Hat Display', sans-serif;
    font-size: 16px;
    background-color: var(--color-paleblue);
}

body::before {
    content: '';
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 50%;
    z-index: -1;
    background-color: var(--color-paleblue);
    background-image: url(images/pattern-background-desktop.svg);
    background-size: cover;
    background-repeat: no-repeat;
    background-position: bottom, 50%, 50%;
}

.container {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%; 
    min-height: 100vh;
}

.card {
    background: var(--color-verypaleblue);
    max-width: 330px;
    border-radius: 20px;
}

.card img {
    width: 100%;
    border-radius: 20px 20px 0 0;
}

.content {
    padding: 30px;
    text-align: center;
}

.content h2 {
    font-weight: 900;
    font-size: 20px;
    margin-bottom: 15px;
}

.content p {
    font-weight: 400;
    font-size: 13px;
    padding: 0 15px;
}

.annual {
    display: flex;
    justify-content: flex-end;
    align-items: center;
    margin-top: 20px;
    width: 100%;
    height: 4rem;
    padding: 5px;
    background-color: hsl(225, 10%, 95%);
    border-radius: 10px;
}

.annual img {
    width: 2.3rem;
}

.annual p {
    font-size: 12.5px;
}

.price {
    margin-right: 2.5rem;
    line-height: 1.2em;
}

p.price-head {
    font-weight: bold;
    color: var(--color-darkblue);
}

p.price-body {
    color: var(--color-desaturatedblue);
}

.annual a p {
    font-weight: bold;
    font-size: 12px;
}

.annual a {
    color: var(--color-brightblue);
    opacity: 1;
}

.annual a:hover {
    opacity: 0.7;
    text-decoration: none;
}

.order-btn {
    margin-top: 1.5em;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 2.5em;
    background-color: var(--color-brightblue);
    border-radius: 10px;
    box-shadow: 0px 5px 18px -2px rgba(0,0,0,0.47);
    opacity: 1;
}

.order-btn a {
    text-decoration: none;
    color: var(--color-paleblue);
    font-size: 12px;
    font-weight: bold;
}

.cancel-btn {
    margin-top: 1em;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 2em;
}

.cancel-btn a {
    text-decoration: none;
    color: black;
    font-size: 12px;
    font-weight: bold;
    opacity: 0.7;
}

.order-btn:hover {
    opacity: 0.7;
}

.cancel-btn:hover a {
    opacity: 1;
}
```

### Useful resources

- [https://w3schools.com] - This helped me for improving my CSS skills and helped me to finihing this project.

## Author

- Frontend Mentor - [https://www.frontendmentor.io/profile/naufalf25]
- Instagram - [https://www.instagram.com/naufal_railfans25/]