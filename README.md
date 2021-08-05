# Frontend Mentor - Tip calculator app solution

This is a solution to the [Tip calculator app challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/tip-calculator-app-ugJNGbJUX). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

- View the optimal layout for the app depending on their device's screen size[Compatible in both Mobile and Desktop]
- See hover states for all interactive elements on the page
- Calculate the correct tip and total cost of the bill per person

### Screenshot
# Desktop Compatable:
![image](https://user-images.githubusercontent.com/60505090/126587630-e5a35e6e-2ec2-4a3b-a10d-9475f2ea89c8.png)
![image](https://user-images.githubusercontent.com/60505090/126587669-f84f454e-5eaf-4229-913c-84fb1033ab71.png)
# Phone/iPad Compatable:
![image](https://user-images.githubusercontent.com/60505090/126587704-4d697bbe-601b-4d87-ab3c-40e09d24f94c.png)
![image](https://user-images.githubusercontent.com/60505090/126587950-d77dc185-3462-44c1-a5ab-8e9bb43203df.png)



### Links

- Solution URL: [FrontEnd Mentor Solution](https://www.frontendmentor.io/solutions/tip-calculator-web-app-using-html-css-and-javascript-PQ9IR6F2l)
- Live Site URL: [Live Site](https://adityasawant21.github.io/Tip-Calculator-Web-App/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- [GitHub Pages](https://pages.github.com/)
- Mobile-first workflow
- Javascript


### What I learned

This are some code snippets that taught me:

```html
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css"
      integrity="sha512-iBBXm8fW90+nuLcSKlbmrPcLa0OT92xO1BIsZ+ywDWZCvqsWgccV3gFoRBv0z+8dLJgyAHIhR35VZc2oM/gI1w=="
      crossorigin="anonymous"
      referrerpolicy="no-referrer"
    />
```
```css
.tip-selector__tips label {
  cursor: pointer;
  background-color: #00494d;
  color: white;
  font-weight: 700;
  width: calc(100% - 30px);
  height: calc(100% - 20px);
  min-height: 36px;
  font-size: 24px;
  padding: 10px 15px;
  border-radius: 5px;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  position: relative;
}

.tip-selector__tips input[type="radio"]:checked + label {
  background-color: #26c0ab;
  color: #00494d;
}
```
```js
//Check to see if this input is empty or less than or equal to 1
    if (numOfPeople === "" || numOfPeople <= 1) {
      numOfPeople = 1;
      document.getElementById("each").style.display = "none";
    } else {
      document.getElementById("each").style.display = "block";
    }
  
    //Calculate tip
    var total = (billAmt * serviceQual) / numOfPeople;
    //round to two decimal places
    total = Math.round(total * 100) / 100;
    //next line allows us to always have two digits after decimal point
    total = total.toFixed(2);
    //Display the tip
    document.getElementById("totalTip").style.display = "block";
    document.getElementById("tip").innerHTML = total;
  
  }
```

If you want more help with writing markdown, we'd recommend checking out [The Markdown Guide](https://www.markdownguide.org/) to learn more.


### Continued development

I want to continue focusing on new technologies like React.js, Node.js, SASS, Bootstrap,etc in future projects.


### Useful resources

- [W3 School](https://www.w3schools.com/css/css3_flexbox_container.asp) - Help me during Centering the flex container.
- [CSS Tricks](https://css-tricks.com/snippets/css/complete-guide-grid/) - Help me for understanding Grid Container.


## Author

- LinkedIn - [Aditya Sawant](https://www.linkedin.com/in/aditya-a-sawant/)
- Frontend Mentor - [@adi123-bit](https://www.frontendmentor.io/profile/adi123-bit)
- Twitter - [@AdityaASawant1](https://www.twitter.com/AdityaASawant1)

## Acknowledgments

I got really good help from Youtube Channels like CodeWithHarry, freeCodeCamp, etc also with Udemy Courses 

