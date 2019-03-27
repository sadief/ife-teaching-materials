## W4D1 Advanced jQuery

Great work tonight everyone! Only one more week left!

Tonight we did a quick review of:

1.  What is the DOM?
    When a browser loads an HTML page, it stores the text of that page as a data structure called the Document Object Model or DOM.

2.  How do we start each jQuery file and why?

```javascript
$(document).ready() {

}
```

We wait until the full HTML page is fully loaded and “ready” to run our jQuery files. The .ready() helper listens for the page to complete loading.

3.  How do you select elements by tag name, class or id using jQuery?

```
Tag: $(‘div’)
Class: $(‘.class-name’)
Id: $(‘#id-name’)
```

4.  If you wanted to create an event listener similar to the ‘:hover’ in CSS, which would you use?
    `mouseenter`

### Adding Children

We can use jQuery to manipulate the elements on our websites in multiple ways.

We will start by looking at adding child elements to the page.

#### Append()

The .append() helper function allows you to add a new element to the DOM at the end of the parent (ie: as the last-child)

```
$('main').append('<p>I go at the end</p>')

$('article').append('<p> I go at the end</p>')
```

#### Prepend()

The .prepend() helper function adds an element to the beginning of the parent’s contents or as the first child.

```
$(‘main’).prepend(“<p> I go at the beginning</p>”)

$(‘article’).prepend(“<h2> I go at the beginning</h2>”)
```

### Adding Siblings

We can also add elements to the page as siblings, instead of children.

#### After and Before

After and Before both create new elements but in different locations, either before or after the selected element.

```
$('li').after("<li>Ghost</li>”)

$('li').before("<li>A new sibling list item</li>")
```

### Removing & Replacing

We can also add elements to the page as siblings, instead of children.

The .remove() helper function will remove the selected element from the page as well as all children/grandchildren and their contents

The .replace() helper function with will completely replace the element selected

```
$(‘.article’).remove()

$(‘li').replaceWith('<p>Hello</p>')
```

### HTML

The HTML function does 2 things:

1. It will provide you with the content of the selected element if not given an argument between the parentheses.
2. Set the content of the selected HTML element;

```
$('h2').html()

$(‘h2’).html("I am the new title”)
```

### Text

The text function does 2 things:

1. It will provide you with the content of the selector element AND all the contents of that element’s children. It will do this for ALL elements that match the selector.
2. Set the content of the selected element;

```
$(‘h2').text()

$(‘h2’).text("I am the new title”)
```

### Links

[Here's](https://www.codecademy.com/learn/learn-jquery) a link to CodeAcademy's jQuery course.

[Here's](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/JSON) a link to MDN's JSON.
