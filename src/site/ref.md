---
title: Reference
layout: layouts/base.njk
---
## HTML / CSS / JavaScript

### 1. HTML [MDN Reference](https://developer.mozilla.org/en-US/docs/Web/HTML)

HTML at its core is structural. It provides a machine readable document called the DOM with what *content* to display. This is central to elements we reference. Simply speaking, most elements require an open (`<>`) and close (`</>`) tag.

Some common reference tags:

- `<!doctype html>`: let's the browser know you're coding in HTML
  - Does not require a closing tag
  - Should always be the first line in a document
- `<html></html>`: This is where all your structure will live (inside the tags)
- `<body></body>`: Anything you want to be directly shown in the browser should be inside the body tags
- `<link href="css/styles.css" type="text/css" />`: a common way to reference a stylesheet
- `<script src="js/app.js" type="text/javascript"></script>`: a common way to reference a javascript file
  - Sometimes loaded near the end of the file to make sure scripts run after all the content has loaded in the page
- `<div></div>`: can contain any type content
- `<h1></h1>`: headings, h1-h6 can be used for different headings/importance
- `<button></button>`: can be use to trigger interactions or form submissions. Within form tags submits forms, otherwise needs some type of listener for an action to happen
- `<ul></ul>`: unordered list, bullet list
- `<ol></ol>`: ordered list, roman numerals or numbers
- `<li></li>`: list items, can be in ul's or ol's but displayed differently based on their parent

A simple HTML file might look like this:

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <link href="css/style.css" type="text/css" />
  <title>COOL WEBPAGE</title>
</head>
<body>
  <!--CONTENT GOES HERE-->
  <div
  <script src="js/app.js" type="text/javascript"></script>
</body>
</html>
```

You can begin to plan your styles by adding classes or ids to your content HTML tags. We can do this very easily.

Of note:

- Classes can be re-used multiple times throughout a page
- ID's should only be used once `<form id="contactForm"></form>`
- You can add multiple classes to a single dom element seperated by a space: `<button class="blue button big"></button>`


----

### 2. CSS [MDN Reference](https://developer.mozilla.org/en-US/docs/Web/CSS)

CSS is the styling and presentational layer, it adds visual richness to the page on top of the structural base of HTML.

Don't forget to normalize your css, or each browser is left to it's default sizing. Normalizing standardizes our styles to be presentationally the same.

To reference the classes and ids that we gave our dom elements earlier, we would use the following:

**HTML**

`<form id="contactform"></form>`

**CSS**
```
#contactform {
  background: pink;
  max-width: 80%;
}
```

**HTML**

`<button class="blue button big"></button>`

**CSS**

```
.blue {
  background: blue;
}
.button {
  color: #fff;
  padding: 15px;
  text-transform: uppercase;
}
```

**HTML**

`<section></section>`

**CSS**

```
section {
  height: 100vh;
  margin: 0 auto;
  width: 100vw;
}
```

----

### 3. JavaScript [MDN Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

Making an HTML page interactive requires Javascript. Using event listeners, functions, variables, we have a technology that can traverse through the DOM and we can listen for events and respond to them using JavaScript.

- Structure
- Defining Variables
  - let : can change throughout the program
  - const : constant, does not change, but is singly defined and it's use does not mutate/change it
  - var : catch all, would stay away from this as it's not a best practice
- Data Types
  - Number : any integer
  - String : anything in quotes, or 
  - Striing literal : anything using back ticks. You can also use variables directly in these strings. e.g. `` `This is ${exclamation}` ``
  - Infinity : causes infiniite loop and will eventually lock the browser
  - Boolean : true (1) or false (0)
  - undefined : not yet used
  - Objects : contain key value pairs
```
const person = {
  firstName: Dan,
  lastName: Leatherman
};
```
  - Arrays
```
const kids = ["Simon", "Leo", "Willa"];
```
- Operators
  - Math with numbers
  - Math with strings
- Comparisons
  - Greater than `>`
  - Less than `<`
  - Equals
    - `==` fuzzy match, strings can match numbers, etc.
    - `===` exact match of type and value
  - Not Equals
    - `!=` fuzzy match
    - `!==` exact match
- Interaction
  - Alert : `alert('message')`
  - Prompt : `prompt('message', callback)`
  - Confirm : `confirm('confirm you want to do this?', callback)`
- Conditionals
```
if (true) {
  // execute this code
}
```
```
if (false) {
  // do this
} else if (true) {
  // do this instead
}
```
  - Logical operators
- Loops
- Switch Statements
- Functions
  - returns
