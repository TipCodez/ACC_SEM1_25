# Frontend Mentor - Chat App CSS Illustration Solution

This is a solution to the [Chat app CSS illustration challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/chat-app-css-illustration-O5auMkFqY). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

## Overview


### Screenshot

![Chat App CSS Illustration](./images/Screenshot%202025-05-14%20013119.png)

### Links

- Solution URL: [Frontend Mentor Solution](https://www.frontendmentor.io/solutions/chat-app-css-illustration-using-html-and-css-with-flexbox-animations-xxXXxxXX)
- Live Site URL: [Live Chat App Illustration](https://your-live-site-url.com)

## My process

I approached this challenge by first analyzing the design files and breaking down the UI into logical components. I started with the HTML structure to ensure all content was properly organized before moving on to styling. I used a mobile-first approach, ensuring the design worked well on smaller screens before adapting it for desktop views.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS animations
- Mobile-first workflow
- Google Fonts - Rubik font family

### What I learned

This project helped me strengthen my CSS skills, particularly in creating complex layouts and realistic UI components. I learned how to:

1. Create a realistic phone UI with proper styling for the notch and header
2. Style chat bubbles with different appearances for sent vs. received messages
3. Implement a gradient background that enhances the overall design
4. Create subtle animations to bring the chat interface to life

One of the most challenging aspects was creating the curved background shapes. I solved this using absolute positioning and border-radius:

```css
.background-shape.left {
  background: linear-gradient(to bottom, var(--light-magenta), var(--light-violet));
  width: 500px;
  height: 700px;
  border-radius: 0 0 250px 250px;
  top: 0;
  left: -100px;
}
```

I'm also proud of the chat message animations that create a staggered loading effect:

```css
@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.message {
  animation: fadeIn 0.3s ease-in-out forwards;
}

.message:nth-child(n) {
  animation-delay: calc(0.1s * n);
}
```

### Continued development

In future projects, I want to focus on:

- Improving my CSS animation skills to create more complex and fluid animations
- Exploring CSS Grid for more complex layouts
- Adding JavaScript functionality to make the chat interface interactive
- Implementing accessibility features to ensure the design is usable by everyone

### Useful resources

- [CSS-Tricks Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - This comprehensive guide helped me understand flexbox layout principles, which were essential for structuring the chat interface.
- [MDN Web Docs on CSS Animations](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Animations/Using_CSS_animations) - This resource was invaluable for implementing the staggered loading animations for the chat messages.
- [Google Fonts](https://fonts.google.com/specimen/Rubik) - The Rubik font family used in this project provides a clean, modern look that matches the design perfectly.

## Author

- Name - Punobyin Raphael Tibil
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Website - [Your Portfolio](https://your-portfolio-website.com)
