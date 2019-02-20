# Intro to Front End - AJAX

**_Set up the Live Stream_**

---

### AJAX & jQuery

What is AJAX? Asynchronous Javascript and XML (markup that defines set of rules for encoding documents). It's basically how we get data from our backend.

---

### jQuery Questions

Any jQuery questions? jQuery review:

- What do we have to have at the top of every jQuery file?

```javascript
$(document).ready(function() {
  //code goes here
});
```

- How do we select elements?

  - tag
  - class
  - id

- hide & show

```JavaScript
$("main").hide(1000);
$("main").show(3000);
```

- slide up & down

```JavaScript
$("main").slideUp(1000);
$("main").slideDown(3000);
```

- delay

```JavaScript
$("main").delay(2000).slideUp(1000);
```

- event listeners

```JavaScript
$('main').click( function() {
  $('.second-square').slideUp(2000);
 })
```

- mouse events

```javascript
$(".first-square").on("mouseenter", function() {
  $(".first-square").hide(1000);
});
```

- forms

```html
<form><input type="text" /> <button type="submit">Submit</button></form>
```

```JavaScript
$("form").submit(function() {
  event.preventDefault();
  console.log($("input").val());
});
```

- append

```javascript
$("main").append("<p>I go at the end</p>");
```

- prepend

```javascript
$("main").prepend("<p> I go at the beginning</p>");
```

- after

```javascript
$("li").after("<li>A new sibling list item</li>");
```

- remove/ replace with

```javascript
$(".article").remove();
```

```javascript
$("li").replaceWith("<p>The Hound</p>");
```

- html

```javascript
$("h2").html();

console.log($("h2").html());
```

- text

```javascript
$(".winterfell").text();

console.log($(".winterfell").text());
```

---

### HTTP

Http stands for HyperText Transfer Protocol, it is the way different computers talk to each other over the internet

---

### CRUD

When we are dealing with data there are four main things we want to 'trigger' in a database:

- Create
- Read
- Update
- Delete

---

### AJAX

AJAX lets us talk to the backend without refreshing our page.

---

### JSON

The structure of data that we get back from an HTTP request

---

### PARAMS

Arguments that we can pass to a backend to receive data

---

### The Request Cycle

So what happens when we go to a URL in a browser? We are making a request. How is that request handled?

---

### Under the Hood

---

### The Flow

GET request
POST request

---

### Get Request with jQuery

So how do we use jQuery to request data?

---

### We have a function called GET

```javascript
$(function() {
  $.get(
    "https://www.thecocktaildb.com/api/json/v1/1/search.php?s=margarita",
    function(data) {
      console.log(data);
    }
  );
});
```

---

### Query Params

Let's break down what parameters happen when we google something

---

### Params Ahoy

We can create query strings from variables so that they can be more dynamic

Which comes in handy when we are grabbing the data from our page… (hint hint)

-
