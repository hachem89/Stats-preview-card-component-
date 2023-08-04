# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- View the optimal layout depending on their device's screen size

### Screenshot

![](./screenshots/desktop-view.png)


### Links

- Solution URL: [Solution](https://github.com/hachem89/Stats-preview-card-component-.git)
- Live Site URL: [Live site](https://hachem89.github.io/Stats-preview-card-component-/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow


### What I learned

- I learned a new measure unit in css which is 'em':
The em unit is relative to the font size of the parent element. If you set an element's font size to 1em, it will inherit the font size of its parent. If the parent's font size is 16px, then 1em will be equivalent to 16px.

- I learned that when it comes to designing the layout for your div containing image, text, and button... , there are   two common approaches: fixed dimensions or using padding and margins. Each approach has its advantages and use cases. Let's go over each one:

  1) **Fixed Dimensions Approach:**
  - In this approach, you explicitly set the height and width of the div container. This means the container will always have the same size, regardless of its content.
  - You can then use CSS positioning (like position: absolute or position: relative) to place the content (image, text, button) inside the div wherever you want it to be.
  - This approach is helpful when you need precise control over the layout, especially if you have a specific design in mind that requires fixed dimensions for the container.


  ```html
  <div class="container">
    <img src="example.jpg" alt="Example Image">
    <p>Some text content goes here.</p>
    <button>Click me</button>
  </div>

  ```
  ```css
  .container {
    position: relative;
    width: 300px; /* Set a fixed width */
    height: 200px; /* Set a fixed height */
  }

  img, p, button {
    position: absolute;
    /* Use top, bottom, left, right properties to position the elements inside the container */
  }

  ```

  2) **Fluid Dimensions with Padding and Margins:**

  - In this approach, you do not set a fixed height and width for the container. Instead, the container will expand or shrink based on its content and any specified padding or margins.
  - You can use margin and padding to create spacing between the elements inside the container, allowing them to naturally flow and position themselves without explicit coordinates.
  - This approach is useful when you want the container to be flexible and adapt to different screen sizes or content lengths. It is also ==great for responsive designs== .

  ```html
  <div class="container">
    <img src="example.jpg" alt="Example Image">
    <p>Some text content goes here.</p>
    <button>Click me</button>
  </div>

  ```
  ```css
  .container {
    padding: 20px; /* Add some padding to create spacing */
  }

  img, p, button {
    margin-bottom: 10px; /* Add margin to create vertical spacing between elements */
  }

  ```
  Ultimately, the choice between the two approaches depends on your project requirements and design preferences. If you want more control and predictability in your layout, go with the fixed dimensions approach. If you prefer a more flexible and responsive layout, use fluid dimensions with padding and margins. Additionally, consider using CSS Flexbox or Grid to further enhance your layout capabilities.

- I learned that the flex property is a shorthand property in CSS that combines three individual properties related to flexible layouts using CSS Flexbox. The three values within the flex property represent the following:
Flex grow, Flex shrink, Flex basis

```css
flex: flex-grow flex-shrink flex-basis;

```
  So, in the case of flex: 1 1 300px;:
  - flex-grow: 1: The item can grow and take up any available space within the flex container.
  - flex-shrink: 1: The item can shrink and reduce its size if there is not enough space in the flex container.
  - flex-basis: 300px: The item's initial size is set to 300 pixels.

The flex property is commonly used to create flexible and responsive layouts using CSS Flexbox. By adjusting these values, you can control how flex items grow, shrink, and initially size themselves within the flex container.

### Useful resources

- [Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - This helped me with the flex property and ordre property 

## Author

- Frontend Mentor - [@hachem89](https://www.frontendmentor.io/profile/hachem89)


