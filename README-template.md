# Frontend Mentor - Results summary component solution

This is a solution to the [Results summary component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/results-summary-component-CE_K6s0maV). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- Adding manual margin and padding
- Making it various device friendly such as mobile

### Screenshot

![Screenshot](image.png)

### Links

- Live Site URL: [Live Server Site](http://127.0.0.1:5500/Result/index.html)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

During this project I have learnt how to code HTML and CSS to make a project . 

Observe below code to make the project.

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <!-- displays site properly based on user's device -->

    <link rel="icon" type="image/png" sizes="32x32" href="favicon-32x32.png" />

    <title>Frontend Mentor | Results summary component</title>

    <link rel="stylesheet" href="style.css">
</head>

<body>
    <div id="wrapper">
        <div class="container">
            <div class="scorecard">
                <div class="box1">
                    <div class="head">Your Result</div>
                    <div class="circle">
                        <div class="score">76</div>
                        <div class="outoff">of 100</div>
                    </div>
                    <div class="box1_text">
                        <h3>Great</h3>
                        <p class="text">
                            You scored higher than 65% of the people who
                            have taken these tests.
                        </p>
                    </div>
                </div>
                <div class="box2">
                    <div class="text">
                        <p class="summary">Summary</p>
                        <div class="subject_score">
                            <div class="reaction">
                                <p class="s1"><img src="icon-reaction.svg" alt="">Reaction</p>
                                <div class="os1">
                                    <p class="b"><b>80</b></p>
                                    <pre> / </pre>
                                    <p class="grey">100</p>
                                </div>
                            </div>
                            <div class="memory">
                                <p class="s2"><img src="icon-memory.svg" alt="">Memory</p>
                                <div class="os1">
                                    <p class="b"><b>92</b></p>
                                    <pre> / </pre>
                                    <p class="grey">100</p>
                                </div>
                            </div>
                            <div class="verbal">
                                <p class="s3"><img src="icon-verbal.svg" alt="">Verbal</p>
                                <div class="os1">
                                    <p class="b"><b>61</b></p>
                                    <pre> / </pre>
                                    <p class="grey">100</p>
                                </div>
                            </div>
                            <div class="visual">
                                <p class="s4"><img src="icon-visual.svg" alt="">Visual</p>
                                <div class="os1">
                                    <p class="b"><b>72</b></p>
                                    <pre> / </pre>
                                    <p class="grey">100</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="button">
                        <button>Continue</button>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <div class="attribution">
        Challenge by
        <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>. Coded by <a
            href="#">Prasanna Pandhare</a>.
    </div>
</body>

</html>
```
```css
@import url(https://fonts.google.com/specimen/Hanken+Grotesk);

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: "Hanken Grotesk", sans-serif;
    font-weight: 500, 700, 800;
    /* src: url(https://fonts.google.com/specimen/Hanken+Grotesk); */
}

#wrapper {
    margin: auto;
    height: 100vh;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    /* border: 1px solid green;
    text-align: center;
    padding-left: 50px;
    padding-top: 50px;
    padding-bottom: 50px;
    padding-right: 50px; */

}

.container {
    display: flex;
    flex-wrap: wrap;
    margin: auto;
    justify-content: center;
    align-items: center;
    /* border: 1px solid red; 
    text-align: center; 
    gap: 10px; 
    width: 1440px;
    padding-left: 400px;
    padding-right: 400px;
    padding-top: 300px;
    padding-bottom: 300px; */
}

.scorecard {
    /* width: 1400px; */
    /* height: 1500px; */
    /* padding-top: 300px; */
    /* padding-bottom: 300px; */
    /* position: relative; */
    display: flex;
    border-radius: 15px;
    box-shadow: 2px 2px 10px #1f1f1f;
    z-index: 9;
}

.box1 {
    /* position: absolute; */
    /* margin: auto; */
    display: flex;
    flex-direction: column;
    width: 50%;
    text-align: center;
    border: 1px solid transparent;
    border-radius: 15px;
    justify-content: center;
    align-items: center;
    background: linear-gradient(hsl(252, 100%, 67%), hsl(241, 81%, 54%));
}

.head {
    font-size: 20px;
    color: hsl(221, 100%, 96%);
    padding: 20px;
    font-weight: 700;
}

.score {
    font-size: 50px;
    font-weight: 800;
    color: hsl(0, 0%, 100%);
}

.outoff {
    font-size: small;
    color: hsl(241, 100%, 89%);
}

.box1_text {
    font-size: 18px;
}

.box1_text h3 {
    padding: 10px;
    color: hsl(0, 0%, 100%);
    padding-bottom: 20px;
}

.box1_text p {
    color: hsl(241, 100%, 89%);
    padding-bottom: 20px;
    font-size: small;
}

.circle {
    border: 1px solid transparent;
    width: 200px;
    height: 200px;
    border-radius: 50%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    background: linear-gradient(hsla(256, 72%, 46%, 1), hsla(241, 72%, 46%, 0));
    text-align: center;
    /* align-items: center; */
}

.text {
    padding-left: 20px;
    padding-right: 20px;
}

.box2 {
    display: flex;
    flex-direction: column;
    width: 50%;
    border: 1px solid transparent;
    padding-left: 30px;
    /* margin: auto; */
}

.button {
    padding-top: 40px;
    padding-bottom: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
}

button {
    border: none;
    border-radius: 30px;
    width: 80%;
    height: 50px;
    color: white;
    background-color: black;
    cursor: pointer;
}

button:hover {
    background: linear-gradient(hsl(252, 100%, 67%), hsl(241, 81%, 54%));
}

.subject_score {
    font-size: 18px;
    font-weight: 500;
    display: flex;
    flex-direction: column;
    gap: 10px;
}

.reaction {
    /* padding-bottom: 5px; */
    /* border: 1px solid black; */
    display: flex;
    justify-content: space-around;
    height: 50px;
    align-items: center;
    border-radius: 15px;
    background: hsla(0, 100%, 67%, 5%);
}

.reaction img {
    /* height: px; */
    width: 25px;
    padding-right: 10px;
}

.memory {
    /* padding-bottom: 5px; */
    /* border: 1px solid black; */
    display: flex;
    justify-content: space-around;
    height: 50px;
    align-items: center;
    border-radius: 15px;
    background: hsla(39, 100%, 56%, 5%);
}

.memory img {
    /* height: 18px; */
    width: 25px;
    padding-right: 10px;
}

.verbal {
    /* padding-bottom: 5px; */
    /* border: 1px solid black; */
    display: flex;
    justify-content: space-around;
    height: 50px;
    align-items: center;
    border-radius: 15px;
    background: hsla(166, 100%, 37%, 5%);
}

.verbal img {
    /* height: 18px; */
    width: 25px;
    padding-right: 10px;
}

.visual {
    /* padding-bottom: 5px; */
    /* border: 1px solid black; */
    display: flex;
    justify-content: space-around;
    height: 50px;
    align-items: center;
    border-radius: 15px;
    background: hsl(234, 85%, 45%, 5%);
}

.visual img {
    /* height: 18px; */
    width: 25px;
    padding-right: 10px;
}

.summary {
    padding-top: 20px;
    padding-bottom: 20px;
    font-weight: 900;
    font-size: 20px;
}

.s1 {
    color: hsl(0, 100%, 67%);
    /* padding-left: 10px; */
}

.s2 {
    color: hsl(39, 100%, 56%);
}

.s3 {
    color: hsl(166, 100%, 37%);
}

.s4 {
    color: hsl(234, 85%, 45%);
}

.os1 {
    display: flex;
    justify-content: space-evenly;
}

.grey,
pre {
    color: grey;
}

.attribution {
    font-size: 12px;
    text-align: center;
}

.attribution a {
    text-decoration: none;
}
```

### Continued development

While working on this project I felt difficulty in making its mobile interface . So I have not added it in this file. I will like to learn media queries after this project.

Please forgive me as I was unable to make mobile preview of this project.

### Useful resources

- [MDN Docs](https://developer.mozilla.org/en-US/) - Helped me in various learnings. 

## Author

- Website - [Prasanna Pandhare](https://www.your-site.com)
- Frontend Mentor - [@Prasannapandhare](https://www.frontendmentor.io/profile/Prasannapandhare)

## Acknowledgments

This project helped me to clarify various concepts of HTML and CSS by using them them practically. 

