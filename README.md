# Frontend Mentor - FAQ accordion solution

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- Hide/Show the answer to a question when the question is clicked
- Navigate the questions and hide/show answers using keyboard navigation alone
- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page

### Screenshot

![](./faq-accordion/assets/images/Frontend%20Mentor%20-%20FAQ%20accordion%20.jpg)

### Links

- Solution URL: [Click here](https://www.frontendmentor.io/solutions/responsive-design-for-faq-accordion-using-htmlcss-and-js-xeY4-b1Pib)
- Live Site URL: [Click here](https://subagas.github.io/faq-accordion/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned
#### JS

```js
function showAnswerOnIcon() {
  this.style.display = 'none';
  const minusIcon = this.nextElementSibling;
  minusIcon.style.display = 'block';
  const questionContainer = this.parentElement.parentElement;
  const answer = questionContainer.lastElementChild;
  answer.style.display = 'block';
}
```
I traversed through DOM elements to get the functionality.

```
const isHidden = window.getComputedStyle(answer).display === 'none';
```
I was not able hide/unhide the elements on the first click every time after I refresh the page. This was happening because JS only reads the inline styles. I overcame it by using getComputedStyle() in JS, it is used to check the computed style of an element which is written externally.

### Continued development

I would learn more into traversing through DOM elements and nodes in JS.

## Author

- Frontend Mentor - [Click here](https://www.frontendmentor.io/profile/SubagaS)
- LinkedIn - [Click here](https://www.linkedin.com/in/subaga/)
