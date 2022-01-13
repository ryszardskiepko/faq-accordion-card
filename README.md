# Frontend Mentor - FAQ accordion card solution

This is a solution to the [FAQ accordion card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/faq-accordion-card-XlyjD0Oam).

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

- View the optimal layout for the component depending on their device's screen size
- See hover states for all interactive elements on the page
- Hide/Show the answer to a question when the question is clicked

### Screenshot

![](./screenshot.jpg)

### Links

- URL: [deployed on Netlify](https://faq-accordion-card-rskiepko.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

To see how you can add code snippets, see below:

```html
<h1>Some HTML code I'm proud of</h1>
```

```css
/*The snippet below helped me to avoid using JS to rotate arrow after clicking on it.*/

@keyframes rotateArrow {
  to {
    transform: rotate(180deg);
  }
}

@keyframes rotateArrowInverse {
  from {
    transform: rotate(180deg);
  }
  to {
    transform: rotate(0deg);
  }
}

details[open] > summary {
  color: $blueGrayishDark1;

  .question-summary__arrow {
    animation: rotateArrow 0.2s ease-out;
    animation-fill-mode: forwards;
  }
}

details > summary {
  .question-summary__arrow {
    animation: rotateArrowInverse 0.2s ease-out;
    animation-fill-mode: forwards;
  }
}
```

If you want more help with writing markdown, we'd recommend checking out [The Markdown Guide](https://www.markdownguide.org/) to learn more.

**Note: Delete this note and the content within this section and replace with your own learnings.**

### Continued development

### Useful resources

- [Example resource 1](<https://developer.mozilla.org/en-US/docs/Web/CSS/color_value/hsl()>) - This article shows some basics about 'hsl()' function.
- [Example resource 2](https://www.quackit.com/css/color/values/css_hsl_function.cfm) - Here are more explanations about 'hsl()' function.
- [Example resource 3](https://developer.mozilla.org/pl/docs/Web/HTML/Element/details) - This article helped me to use the 'details' and 'summary' tags, so I was able to prevent the use of Javascript to expand the response content when clicking on a question.
- [Example resource 4](https://codepen.io/codeseries09/pen/poowRqK) - Here is another article showing the solution to the problem described in the point above.

## Author

- Frontend Mentor - [@ryszardskiepko](https://www.frontendmentor.io/profile/ryszardskiepko)
- Github - [@ryszardskiepko](https://github.com/ryszardskiepko)

## Acknowledgments
