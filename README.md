# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. It was coded by https://github.com/dbustamanter

## Overview
This challenge helped me to practice HTML + CSS coding. Using some flexbox layout, that make the design easier, and usign the Mobile-first workflow.
### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot
![Alt text](/design/solution/Screen%20Shot%202022-05-17%20at%2020.17.59.png "Responsive deploy")
![Alt text](/design/solution/Screen%20Shot%202022-05-17%20at%2020.20.45.png "Mobile hover")
![Alt text](/design/solution/Screen%20Shot%202022-05-17%20at%2020.23.03.png "Web deploy")
![Alt text](/design/solution/Screen%20Shot%202022-05-17%20at%2020.23.12.png "Web hover")

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

In this challenge i've learned to make a hover effect, using transitions and overlay images:

/*HOVER EFFECT*/
.fade {
    position: relative;
    width: auto;
    height: auto;
  }
  
  .image {
    opacity: 1;
    display: block;
    transition: .5s ease;
    backface-visibility: hidden;
  }
  
  .middle {
    position: absolute;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 17rem;
    height: 17rem;
    background-color: rgba(0, 255, 247, 0.5);
    border-radius: .5rem;
    transition: .5s ease;
    opacity: 0;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%)
  }
  
  .fade:hover .image {
    opacity: 0.8;
  }

  .fade:active .image{
      opacity: 0.8;
  }
  
  .fade:hover .middle {
    opacity: 1;
  }

  .fade:active .middle{
      opacity: 1;
  }
  
  .eye {
    color: #ffff;
    padding: 16px 32px;
    background-color: none;
  }
  /*---------------------------------------------*/


### Useful resources

- [Overlay effects](https://www.w3schools.com/howto/howto_css_image_overlay.asp) - This helped me for Hover effects on the NFT's image.

## Author

- LinkedIn - [Diego Bustamante R.](https://www.linkedin.com/in/dbustamanter/)
- Frontend Mentor - [@dbustamanter](https://www.frontendmentor.io/profile/dbustamanter)

## Got feedback for us?

We love receiving feedback! We're always looking to improve our challenges and our platform. So if you have anything you'd like to mention, please email hi[at]frontendmentor[dot]io.

This challenge is completely free. Please share it with anyone who will find it useful for practice.

**Have fun building!** 🚀
