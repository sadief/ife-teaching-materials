# Intro to Front End - Advanced JQuery

**_Set up the Live Stream_**

---

### Front End Fundamentals

How's JQuery going?

---

### Advanced jQuery

Today’s Objectives:

- Access and loop over deeply nested data from within a JavaScript object
- Manipulate elements on your page with jQuery methods
- Create a grid-like display of data by combining these two actions

**_Starter Code_**

```HTML
<!DOCTYPE html>
<html>
  <head>
    <title>Advanced JQuery</title>
    <link rel="stylesheet" href="./index.css" type="text/css">
    <link href="https://fonts.googleapis.com/css?family=Montserrat:400,700" rel="stylesheet">
  </head>
  <body>
    <header>
      <h1>Advanced JQuery</h1>
    </header>
    <main>
      <article class="article">
        <h1>Winter is Coming</h1>

        <p>You know nothing Jon Snow</p>
      </article>

      <article class="article">
        <h2>A Lannister always pays his debts</h2>

        <h6>Arya is the best</h6>

        <p>Joffrey sucks</p>

        <ul>
          <li>Sansa is boring</li>

          <li>Jamie and Brienne need their own show</li>
        </ul>
      </article>
    </main>

    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
    <script src="./index.js"></script>
 </body>
</html>
```

```css
html {
  font-family: "Montserrat", sans-serif;
  background-color: #172a3a;
  color: #75dddd;
}

header {
  color: #75dddd;
}

body {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  color: #508991;
}

main {
  display: flex;
  justify-content: center;
  align-items: center;
}

article {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin: 25px;
  padding: 20px;
  background-color: #004346;
  font-size: 24px;
}

h2,
h6 {
  margin-bottom: 15px;
}
```

---

### Review

Javascript objects - create an object and retrieve data from it.

Jquery basics:

**_What is the DOM?_**

When a browser loads an HTML page, it stores the text of that page as a complicated data structure called the Document Object Model or DOM.

**_How do we start each jQuery file and why?_**

`$(document).ready()`

We wait until the full HTML page is fully loaded and “ready” to run our jQuery files. The .ready() helper listens for the page to complete loading

**How do you select elements by tag name, class or id using jQuery?**

- Tag: `$(‘div’)`
- Class: `$(‘.class-name’)`
- Id: `$(‘#id-name’)`

**If you wanted to create an event listener similar to the ‘:hover’ in CSS, which would you use?**

`mouseenter`

---

### Advanced jQuery

Today’s objective is to learn how to create and manipulate the elements on our page.

These tools are especially useful when a user makes a request for information and you need to display the results of that query.

---

### Adding Children

We can use jQuery to manipulate the elements on our websites in multiple ways.

We will start by looking at adding child elements to the page.

---

### Append

The .append() helper function allows you to add a new element to the DOM at the end of the parent (ie: as the last-child)

**_Live Code_**

```javascript
$("main").append("<p>I go at the end</p>");
```

```javascript
$("article").append("<p> I go at the end</p>");
```

---

### Prepend

The .prepend() helper function adds an element to the beginning of the parent’s contents or as the first child.

**_Live Code_**

```javascript
$("main").prepend("<p> I go at the beginning</p>");
```

```javascript
$("article").prepend("<h2> I go at the beginning</h2>");
```

---

### Adding Siblings

We can also add elements to the page as siblings, instead of children.

After and Before both create new elements but in different locations, either before or after the selected element.

**_Live Code_**

```javascript
$("li").after("<li>A new sibling list item</li>");
```

```javascript
$("li").before("<li>A new sibling list item</li>");
```

---

### Removing and Replacing

jQuery gives us helper functions that remove elements from the page and others to replace

---

### Remove Replace

The .remove() helper function will remove the selected element from the page as well as all children/grandchildren and their contents

The .replace() helper function with will completely replace the element selected

**_Live Code_**

```javascript
$(".article").remove();
```

```javascript
$("li").replaceWith("<p>The Hound</p>");
```

---

### HTML

The HTML function does 2 things:

    1. It will provide you with the content of the selected element if not given an argument between the parentheses;
    2. Set the content of the selected HTML element;

**_Live Code_**

```javascript
$("h2").html();

console.log($("h2").html());
```

```javascript
$("h2").html(
  "Why is Robb Scottish and the rest of his family is from Yorkshire?"
);
```

---

### Text

The text function does 2 things:

1. It will provide you with the content of the selector element AND all the contents of that element’s children. It will do this for ALL elements that match the selector;

2. Set the content of the selected element;

**_Live Code_**

```javascript
$(".winterfell").text();

console.log($(".winterfell").text());
```

```javascript
$(".winterfell").text(
  "Why does everyone have perfect eyebrows? Where are they getting tweezers?"
);
```

---

### JSON

JSON stands for Javascript Object Notation and it is a syntax for storing and exchanging data.

When data is returned to the browser from database requests, it is often in JSON format

---

### JSON

What does this look like?

We want them to notice that is is simply in javascript object notation.

You will be using this in the compass exercise today - you'll want to place it at the top of your file and store it as a variable to use.

### Reminders

- Record [Attendance](https://docs.google.com/spreadsheets/d/1e4Umh2ctkuot1fTwZQ43NxlWMvzsz2c-eGYQ_aVB5RA/edit#gid=1835992904)
- Upload lecture
- Send out Notes
- Log hours on Clocktower
