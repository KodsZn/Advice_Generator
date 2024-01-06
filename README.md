# Frontend Mentor - Advice generator app solution

This is a solution to the [Advice generator app challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/advice-generator-app-QdUG-13db). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)


## Overview

### The challenge

Users should be able to:

- View the optimal layout for the app depending on their device's screen size
- See hover states for all interactive elements on the page
- Generate a new piece of advice by clicking the dice icon



### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here]([https://your-live-site-url.com](https://lustrous-pegasus-d9d595.netlify.app))

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox


```css
.proud-of-this-css {
  position: absolute;
      left: 44%;
      top: 93%;
}
```
```js
  <script>
          function generateAdvice() {
              fetch('https://api.adviceslip.com/advice')
                  .then(response => response.json())
                  .then(data => {
                      document.getElementById('advice').textContent = data.slip.advice;
                      document.getElementById('id').textContent = data.slip.id;


            });
    }

              document.addEventListener('DOMContentLoaded', function() {
                  generateAdvice();
                  document.getElementById('adviceBtn').addEventListener('click', generateAdvice);
              });
       </script>

```

### Useful resources

- [w3school](https://www.w3schools.com/js/js_events.asp) - This helped me for creating the js functions to get my adices.


## Author

- Frontend Mentor - [@KodsZn](https://www.frontendmentor.io/profile/KodsZn)

