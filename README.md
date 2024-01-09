# Frontend Mentor - Advice generator app solution

## Table of contents

  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
  - [Built with](#built-with)
  - [Useful resources](#useful-resources)
- [Author](#author)

### The challenge

Users should be able to:

- View the optimal layout for the app depending on their device's screen size
- See hover states for all interactive elements on the page
- Generate a new piece of advice by clicking the dice icon

### Screenshot
![adice-generator screenshot](https://github.com/KodsZn/Advice_Generator/assets/139270026/99285f2d-ced2-4e3a-bd14-e059661f1496)

### Links

- Solution URL: [Add solution URL here]([https://your-solution-url.com](https://www.frontendmentor.io/solutions/advicegenerator-xHPkOj12ir))
- Live Site URL: [Add live site URL here]([https://your-live-site-url.com](https://lustrous-pegasus-d9d595.netlify.app))

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox


```css
.attribution {
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

