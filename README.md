<!-- 
---
title: Persisting Form Input with jQuery and Browser Storage
type: lesson
duration: "1:00"
creator:
    name: Ben Hulan
    city: SF
competencies: Front-end intro
adapted by: 
    name: Zeb Girouard
    city: DEN
---
 -->

<!--WDI6 11:18 -->
<!--WDI5 11:10 -->

<!-- Hook: So...you're filling out a form for something: taxes, registration, or a sign-up for a website.  You realize you made a mistake, so you hit the back button...but that takes you all the way to the beginning.  And worse yet, all your information is now gone.  You have to start all over again. Raise your hand if this has happened to you.  

Today we will talk about one way to resolve this headache, with localStorage.

Another headache you may be familiar with is from the LOTR lab.  Remember having to remember all those complex commands for selecting IDs, classes, and attributes?  

Well, with jQuery we'll make that process a lot easier.
-->

# Persisting Form Input with jQuery and Browser Storage

<!--11:13 WDI4 -->
<!--Actually 11:17 -->
<!-- 5 minutes -->

### Objectives
*After this lesson, students will be able to:*

- **Import** jQuery to a webpage
- **Construct** a jQuery selector
- **Create** HTML forms and store user input in the browser
- **Read** and **write** data with localStorage and sessionStorage
- **Understand** the pros and cons of using built-in browser storage

### Preparation
*Before this lesson, students should already be able to:*

- **Write** basic HTML/CSS
- **Read** and **write** basic vanilla Javascript

<!-- CFU Fist-to-five on these concepts -->

### Independent Practice

<!--WDI6 11:23 turning over to devs -->
<!--Actually 11:21 for direction giving, 11:23 for start -->
<!--WDI4 11:17 after directions done -->
<!--WDI5 11:15 turning over to devs -->
<!-- 10 minutes -->

Take a minute to think out the following steps.  In pairs, complete the following steps:

 - Create a boilerplate `index.html` page (remember the `<h` + `tab` trick in Sublime?)
 - Import jQuery *Hint: you can use a link from the [previous jQuery lesson](https://github.com/den-materials/intro-jquery)*
 - Create a heading tag (h1, h2, or h3)
 - Give it a class
 - Create an inline-script tag below your jQuery import
 - Use jQuery to select this heading, and change its color

Bonus:

 - If you have time, use jQuery to select another element, and change its positioning or size

<!--11:34 WDI6 -->
<!--WDI5 11:25 -->
<!--11:29 WDI4 -->
<!--Actually 11:33 -->
<!-- 5-10 minutes -->

## Why do we need localStorage?
In this Unit we will be building Browser games with HTML, CSS and client-side JavaScript. Although we are not yet ready to connect a database on the backend or store data on a server, the browser offers the ability to persist data locally using `sessionStorage`, `localStorage` and some other options we may explore later in the course.

Creating a game, you may wish to allow your users to store their names and high scores, or keep track of some other simple data.

[Here](https://developer.mozilla.org/en-US/docs/Web/API/Storage) is a look at some documentation for the Web Storage API.

### localStorage vs sessionStorage

`localStorage` and `sessionStorage` both extend Storage. There is no difference between them except for the intended "non-persistence" of `sessionStorage`.

That is, the data stored in `localStorage` persists until explicitly deleted. Changes made are saved and available for all current and future visits to the site.

For `sessionStorage`, changes are only available per window (or tab in browsers like Chrome and Firefox). Changes made are saved and available for the current page, as well as future visits to the site on the same window. Once the window is closed, the storage is deleted.

## Warm-up

<!--WDI6 11:39 -->
<!--Actually 11:40 -->
<!-- 15 minutes -->

Before we begin, let's look at the files in this repository. 
`sessionStorage.html` is the most basic. We will go through this line-by-line in class.
`localStorage1.html` does the same thing, but it adds the clear button.
`localStorage2.html` takes things a bit farther. Take a look at the code and _without opening it in the browser_ see if you can explain what's happening.

<!--11:44 after going through localStorage1.html and sessionStorage.html, then turning over to devs to talk over 2 and 3.html in pairs -->
<!--WDI6 11:49 turning over to devs for last two, coming back 12:01  -->

<!-- CFU: Think-pair-share to explain what's happening on 2nd file -->

Let's brainstorm some other tasks we can accomplish with localStorage or sessionStorage

## Group Exercise:

<!--WDI5 11:50 -->
<!--WDI4 11:54 -->
<!--Actually 11:57 -->
<!--20-25 minutes -->

- Work with your partners
- Figure out something to keep track of on a simple single-page web app
- Create an HTML Form
- Save the info to localStorage
- Feel free to "borrow" liberally from the example code in the repo, _but no copy-paste_

**Hint:** Form submission will usually try to direct a user to a different page.  You may want to look into [preventDefault](https://api.jquery.com/event.preventdefault/) to prevent this.

_Remember: `localStorage` and `sessionStorage` only store strings, so you may need to `parseInt()` if you need to do anything with the user data after it has been entered._

<!--WDI5 12:15 -->
<!--WDI6 12:30 -->

## Resources:

[jQuery Intro on W3Schools](http://www.w3schools.com/jquery)

## Licensing
All content is licensed under a CC­BY­NC­SA 4.0 license.
All software code is licensed under GNU GPLv3. For commercial use or alternative licensing, please contact legal@ga.co.
