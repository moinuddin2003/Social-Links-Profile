# Frontend Mentor - Social links profile solution

This is a solution to the [Social links profile challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

Users should be able to:

- See hover and focus states for all interactive elements on the page

### Screenshot

![](./screenshot.jpg)

### Links

- **Frontend Mentor:** [@moinuddin2003](https://www.frontendmentor.io/profile/moinuddin2003)
- **GitHub:** [@moinuddin2003](https://github.com/moinuddin2003)

## My process

### Built with

- Semantic HTML5 markup
- CSS3 (Flexbox, spacing, transitions)

### What I learned

#### 1. Spacing with `gap` property

I used the `gap` property in two key places:
- On `.card` with `flex-direction: column` to create space between all child elements
- On `.links ul` to create consistent space between each link button

This was much cleaner than adding individual margins and taught me that `gap` is the modern way to control spacing in Flexbox.

```css
.card {
  display: flex;
  flex-direction: column;
  gap: 1rem;  /* space between all children */
}

.links ul {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;  /* space between links */
}
```

#### 2. How `opacity` affects elements

I discovered that setting `opacity: 0.8` on the quote paragraph made the entire element slightly transparent. This creates visual hierarchy and makes text feel less prominent while keeping it readable.

```css
p.quote {
  font-size: 0.8rem;
  font-style: italic;
  opacity: 0.8;
}
```

#### 3. Styling interactive elements (links as buttons)

I learned how to turn plain links into styled buttons by combining CSS properties:
- `display: block` – Makes the link fill full width
- `padding` – Adds space inside for breathing room
- `background` color – Makes it look clickable
- `border-radius` – Rounded corners
- `transition: background 0.2s` – Smooth hover effect
- `:hover` and `:focus` – Visual feedback for users

```css
.links li a {
  display: block;
  background: hsl(0, 0%, 17%);
  padding: 0.75rem 1rem;
  border-radius: 0.5rem;
  transition: background 0.2s;
}

.links li a:hover,
.links li a:focus {
  background: hsl(0, 0%, 25%);
}
```

#### 4. Flexbox for page layout

Using `display: flex` with `justify-content: center` and `align-items: center` on the body centred the card vertically and horizontally. Combined with `min-height: 100vh`, this kept the card centred on any screen size.

### Continued development

I want to build on these CSS fundamentals and move toward **React and Next.js full-stack projects**. The layout, spacing, and interactive styling patterns I learned here will transfer directly to larger applications.

### Useful resources    

- **GitHub Copilot** - Helped me think through CSS properties and debug styling. It also helps me in writing Readme.md
- **Frontend Mentor** - Great platform for learning by building real projects

## Author

- **GitHub:** [@moinuddin2003](https://github.com/moinuddin2003)
- **Frontend Mentor:** [@moinuddin2003](https://www.frontendmentor.io/profile/moinuddin2003)
- **LinkedIn:** [Muhammad Moinuddin](https://www.linkedin.com/in/muhammad-moinuddin-a84698204/)
- **Instagram:** [@asalnaturals.co](https://www.instagram.com/asalnaturals.co/)
- **Facebook:** [Muhammad Moinuddin](https://www.facebook.com/profile.php?id=61565963042735)
