## W4D1 Intro to JQuery

Hey everyone! Great work tonight! So today we did a review of:

- Console Logs: a helper function that prints out to the console
- Data Types: the values we use in javascript are all of a type and these are
- Numbers: we can add, subtract, multiply and divide numbers in JS
- Strings: often represent names, email addresses in code
- Booleans: values that are true or false
- Variables: store values for reuse
- Functions: help us store instructions and actions for reuse
- If statements: allow our code to do different things based on conditions
- Objects: organized sets or related information stored as key-value pairs. We can use dot or bracket notation to retrieve values
- Arrays: lists or collections of stored values. Bracket notation is used to retrieve values
- Loops: allow us to repeat the same action or code to each item in an array or object;

Then we learned some jQuery!

### The DOM

When a browser loads an HTML page, it stores the text of that page as a tree-like data structure called the Document Object Model or DOM. Changing a page’s style or markup in dev tools is accessing and changing the DOM. We use Javascript to access and change that structure.

### What is JQuery?

jQuery is a very popular javascript library for making webpages interactive. It provides developers with many “helper methods” that perform tasks like hiding elements when they are clicked.

A library is just a file we can put in our apps that contain a bunch of helpful functions that make common tasks easier to execute.

### Adding Javascript and JQuery

To add javascript and jQuery, we put the following just above the `</body>` tag in our HTML.

```javascript
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
<script type="text/javascript" src="./index.js"></script>
```

### Selecting Elements in jQuery

We can select elements by using the same selectors we use in CSS:

Example:

```javascript
1. Tag Name:
	$(‘h1)
2. Class:
	$(‘.first-square’)
3.  Id:
	$(‘#content-box’)
4. Nested Tag Name
  $('section p span')
```

### jQuery Animations

#### Show / Hide

Show and hide will either display the selected element or hide it. The value between parentheses is the duration of the animation and as always, we start with the ‘ \$ ‘ jQuery shortcut.

Example:

```
1. Hide ‘main’:
		$('main').hide(1000);

2. Show ‘main’:
		$(‘main').show(3000);
```

#### Slide Up & Down

These helpers also show & hide elements by sliding them in or out from the top of the screen.

Example:

```
1. Slide up ‘main’:
   $(‘main').slideUp(1000);

2. Slide down ‘main’:
   $(‘main').slideDown(3000);
```

#### Delay

All of the animations we have seen so far happen as soon as we refresh the page. They delay helper takes a duration argument and waits to start the queued animations for that amount of time.

Example:

```
$(‘main’).delay(2000).slideUp(1000);

$(‘main’).hide(1000).delay(2000).slideDown(3000);

```

### Event Listeners

So far, all the animations we’ve used have happened as soon as well refresh the page. Usually, we want animations or interactions to run when an ‘event’ happens.

Events are form submissions, button clicks, hovering over elements and many more.

We can use jQuery to listen for these events and then run some code when they occur.

#### Click Events

To attach a click event to an element, use the .click() helper which accepts a function as an argument.  
That function will contain the action you want performed after a click event has occurred.

Example:

```
$('main').click( function() {
            $('.second-square').slideUp(2000);
 })

```

#### Mouse Events

Another common event to attach actions to are those caused by the mouse entering or leaving the space an element takes up.  
These are ‘mouseenter’ and ‘mouseleave’. These events are similar to the CSS ‘ :hover’ state, we are now using javascript to override the browser’s default styling!
To demonstrate these events, we will be using a condensed version of the jQuery event helper function which uses the .on() helper function. It takes an event name as a string and then another function will describes the actions to be performed.

Example:

```
1. Mouse Enter

		$('.first-square').on('mouseenter', function() {
			$('.first-square').hide(1000);
});


2. Mouse Leave

		$(‘.square-two’).on(‘mouseenter’, function() {
		    $(‘.square-two).hide(1000).show(2000);
		});


```

### Forms

In our projects, we will be using a small form to submit a query and the external data sources will return data that matches.
When we submit a form, all the data the user has entered is gathered up and submitted to the backend.

There are a million ways to handle form submissions but we will be using jQuery.

To create a form, HTML has a semantic <form> tag!

Inputs are the tags which will actually collect the user’s input. We change the type attribute to change the type of input we are using. We will be using ‘text’, the most common.

```html
<form><input type="“text”" /> <button type="“submit”">SUBMIT</button></form>
```

We are going to use jQuery to handle form submission and turn off some of the browser’s default behaviour.

jQuery, of course, has a helper function for this called, .submit() which accepts a function containing the actions to be performed.
On submit, the browser will refresh the page so we add event.preventDefault() to prevent the default behaviour of the submit event.

In the code example, we use another helper function, .val(), which collects the content the user inputted.

```javascript
$("form").submit(function() {
  event.preventDefault();

  console.log($("input").val());
});
```

### Resources

[MDN “First HTML Form” tutorial](https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms/Your_first_HTML_form)

[jQuery Documentation](http://api.jquery.com/)

[Target Elements, jQuery Practice](https://learn.freecodecamp.org/front-end-libraries/jquery/target-html-elements-with-selectors-using-jquery/)

[Use jQuery to modify page](https://learn.freecodecamp.org/front-end-libraries/jquery/use-jquery-to-modify-the-entire-page/)
