# Frontend Mentor - Blog Preview Card Solution

This is my solution to the [Blog Preview Card Challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). This challenge helped me practice my HTML, CSS, and JavaScript skills by building a realistic project.

## Table of Contents

- [Overview](#overview)
  - [The Challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My Process](#my-process)
  - [Built With](#built-with)
  - [What I Learned](#what-i-learned)
  - [Continued Development](#continued-development)
  - [Useful Resources](#useful-resources)
- [Author](#author)

## Overview

### The Challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![Design preview for the Blog Preview Card](./preview.jpg)

### Links

- **Solution URL:** [Solution URL](https://github.com/saadoonahmedkhan/blog-preview-card-main)
- **Live Site URL:** [Live Site URL](https://saadoonahmedkhan.github.io/blog-preview-card-main/)

## My Process

### Built With

- **Semantic HTML5 markup**
- **CSS custom properties**
- **Flexbox & CSS Grid**
- **Mobile-first workflow**
- **JavaScript for interactivity**
- **jQuery (if needed)**

### What I Learned

This project helped me improve my understanding of **responsive design**, **CSS layout techniques**, and **hover effects**. Below are some key takeaways:

#### **1. Using CSS Grid & Flexbox for Layout**
I structured the **blog preview card** using a combination of **CSS Grid** and **Flexbox**, ensuring proper alignment and responsiveness.

```css
figure {
  display: flex;
  flex-direction: column;
  align-items: center;
}
```

#### **2. Implementing Hover Effects with `::after`**
I added a **brightness effect on hover** using `::after`, making the card stand out.

```css
figure::after {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: hsla(0, 0%, 100%, 0.3);
  opacity: 0;
  transition: opacity ease-in-out 0.5s;
}

figure:hover::after {
  opacity: 0.8;
}
```

#### **3. Adding Hover & Active Effects on `h1`**
I applied a smooth **color transition** to `h1` when hovered or clicked.

```css
h1 {
  transition: color 0.5s ease-in-out;
}

h1:hover,
h1:active {
  color: gold;
}
```

#### **4. Mobile-First Approach**
I structured my CSS using **media queries**, ensuring that the card looks great on both **mobile (320px)** and **desktop (1440px)**.

```css
@media screen and (min-width: 320px) and (max-width: 550px) {
    figure {
        width: 15rem;
        height: auto;
    }
}
```

#### **5. JavaScript & jQuery for Future Interactions**
Although **no complex JS functionality was required**, I included `index.js` and `jquery.js` for potential **interactivity** (like animations or API calls in the future).

### Continued Development

I want to continue improving:
- **Accessibility (ARIA roles, keyboard navigation)**
- **Advanced animations using CSS and JavaScript**
- **Better performance optimizations for responsiveness**

### Useful Resources

- [CSS Tricks - Flexbox Guide](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - Helped me structure the layout effectively.
- [MDN Web Docs - Grid Layout](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout) - Improved my understanding of Grid systems.

## Author

- Frontend Mentor - [@saadoonahmedkhan](https://www.frontendmentor.io/profile/saadoonahmedkhan)
- Twitter - [@saadoonahmedkhan](https://www.twitter.com/saadoonahmedkhan)

---

Thanks for checking out my solution! Let me know if you have any feedback. 🚀

