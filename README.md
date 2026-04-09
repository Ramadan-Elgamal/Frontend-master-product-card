# Frontend Mentor - Product Preview Card Component

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

### The challenge

This challenge was to build a responsive product preview card component for a fragrance brand. The goal was to create a clean, modern card that displays product information with proper styling and responsive design.

Users should be able to:

- View the optimal layout depending on their device's screen size (mobile: 375px, desktop: 1440px)
- See hover and focus states for interactive elements
- Add the product to their cart via the call-to-action button

### Screenshot

![Product Preview Card Component](./screenshot.png)

### Links

- Solution Repository: [Frontend-master-product-card](https://github.com/Ramadan-Elgamal/Frontend-master-product-card)
- Challenge URL: [Frontend Mentor Challenge](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa)

## My process

### Built with

- **Semantic HTML5** - Using meaningful markup with `<article>`, `<picture>`, and proper heading hierarchy
- **CSS custom properties** - Variables for colors, fonts, and sizing for better maintainability
- **Flexbox** - For layout alignment and spacing (especially the price and button container)
- **Responsive design** - Mobile-first workflow with media queries for tablet/desktop views
- **Google Fonts** - Montserrat (body) and Fraunces (headings) for typography
- **BEM naming convention** - For organized and scalable CSS classes

### What I learned

Through building this component, I reinforced several key concepts:

1. **Responsive Images with `<picture>`** - Using the `<picture>` element to serve different images based on screen size, improving performance and user experience

   ```html
   <picture class="product__img">
     <source
       srcset="./images/image-product-desktop.jpg"
       media="(min-width: 600px)"
     />
     <img
       src="./images/image-product-mobile.jpg"
       alt="Gabrielle Essence Eau De Parfum"
     />
   </picture>
   ```

2. **CSS Custom Properties** - Leveraging CSS variables for consistent theming and easier maintenance across the component

   ```css
   :root {
     --clr-primary: hsl(158, 36%, 37%);
     --clr-primary-dark: hsl(158, 42%, 18%);
     --ff-accent: "Fraunces", serif;
     --ff-base: "Montserrat", sans-serif;
   }
   ```

3. **Accessibility considerations** - Including proper alt text for images and ensuring focus states are visible for keyboard navigation

4. **Flexbox for complex layouts** - Using `gap`, `align-items`, and `justify-content` for precise control over spacing and alignment

### Continued development

Areas I'd like to explore in future projects:

- **CSS Grid** - While Flexbox handled this well, practicing Grid for more complex multi-section layouts
- **Animation and transitions** - Adding smooth CSS transitions for hover states and state changes
- **Advanced responsive techniques** - Experimenting with container queries for even more robust responsive design
- **Form validation** - When the cart functionality becomes interactive, implementing proper form handling
- **Testing** - Learning to write tests for component behavior and accessibility

### Useful resources

- [MDN: Responsive images](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images) - Excellent guide on using `<picture>` and `srcset`
- [MDN: CSS Custom Properties](https://developer.mozilla.org/en-US/docs/Web/CSS/--*) - Comprehensive reference for CSS variables
- [CSS-Tricks: A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - Visual and clear explanations of Flexbox properties
- [Figma to Code Community](https://www.frontendmentor.io/community) - Helpful feedback and solutions from other developers

## Author

- Frontend Mentor - [@Ramadan-Elgamal](https://www.frontendmentor.io/profile/Ramadan-Elgamal)
- GitHub - [Ramadan-Elgamal](https://github.com/Ramadan-Elgamal)