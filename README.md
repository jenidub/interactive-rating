# Frontend Mentor - Interactive Rating Component by JeniDub
This is a solution to the [Interactive rating component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/interactive-rating-component-koxpeBUmI). Frontend Mentor challenges help you improve your coding skills by building realistic projects

## Table of Contents
- [Overview](#overview)
  - [The Challenge](#the-challenge)
  - [Screenshot Library](#screenshot-library)
  - [Links](#links)
- [My Process](#my-process)
  - [Project Tech Stack](#project-tech-stack)
  - [What I Learned](#what-i-learned)
  - [Useful Resources](#useful-resources)
- [Author Info](#author-info)

## Overview
The goal of the Interactive Rating Component project is to allow users to rate a project and see the result along with a thank you message that is responsive to the size of the device screen.

### The Challenge
Users should be able to:
- View the optimal layout for the app depending on their device's screen size
- See hover states for all interactive elements on the page
- Select and submit a number rating
- See the "Thank you" card state after submitting a rating

### Screenshot Library
[Desktop Interactive Screenshot](./images/rating-desktop-interactive.png)
[Desktop Thank You Screenshot](./images/rating-desktop-thankyou.png)
[Mobile Interactive Screenshot](./images/rating-mobile-interactive.png)
[Mobile Thank You Screenshot](./images/rating-mobile-thankyou.png)

### Links
- Solution URL: [Solution URL](https://github.com/jenidub/interactive-rating)
- Live Site URL: [Live Site URL](https://jenidub.github.io/interactive-rating/)

## My Process
I began the development process with the mobile design first to ensure the component fit properly. I did the HTML and CSS first then began to think about the logic needed to switch from the rating to the thank you message using Javascript. After completing the mobile design, I designed the desktop version and adjusted the HTML and CSS to look good on all size screens.

### Project Tech Stack
- HTML
- CSS
- Flexbox
- CSS Grid
- Mobile-first workflow
- In-line Javascript
- DOM Manipulation

### What I Learned
I figured out how to use in-line Javascript properly to switch between two displays. Here is a sample of the in-line Javascript I used for this project: 

  //After Submit Button Clicked
  function changeDisplay() {
    thankYouPage.style.display = "block";
    ratingPage.style.display = "none";
    if(userRating.innerHTML === "") {
      document.querySelector("#selection-display").remove();
      document.querySelector("#selection-text-h2").innerHTML = "No Rating Was Given";
      document.querySelector("#selection-text-p").innerHTML = "Please use the button below to submit a rating";
    }
  }

### Useful Resources
- [Geeks for Geeks Inline JS Tutorial](https://www.geeksforgeeks.org/how-does-inline-javascript-work-with-html/) - This provided a great sample of how to write inline Javascript effectively in a project
- [Wes Bos Javascript 30](https://github.com/wesbos/JavaScript30) - This course provides many examples of using inline Javascript that provided inspiration for this project

## Author Info
- JeniDub Website - [@JeniDub GitHub Profile](https://github.com/jenidub)
- Frontend Mentor - [@jenidub](https://www.frontendmentor.io/profile/jenidub)
