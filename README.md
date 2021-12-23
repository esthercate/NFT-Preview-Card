# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](./screenshot.jpg)

Find the final solution folder, containing the screenshots of the finished project. 

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS and SCSS
- Mobile-first workflow

### What I learned

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

To see how you can add code snippets, see below:


```css
.card-header {
    position: relative;
    cursor: pointer;
    width: 100%;
    

    .card-image {
        width: 100%;  
        background-size: cover;
        overflow: hidden;
        border-radius: 8px;
    }
}

.card-header::after {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    height: 99%;
    width: 100%;
    background: color(primary-cyan);
    border-radius: 8px;
    opacity: 0;
    visibility: hidden;
    transition: opacity 0.5s ease;

}

.card-header:hover::after {
    opacity: .5;
    visibility: visible;
}

img.icon-view {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    height: 50px;
    width: 50px;
    transition: opacity 0.2s ease;
    z-index: 9;
    opacity: 0;
    visibility: hidden;
}

.card-header:hover img.icon-view {
    opacity: 1;
    visibility: visible;
}

```

## Author

- Frontend Mentor - [@esthercate](https://www.frontendmentor.io/profile/esthercate)


