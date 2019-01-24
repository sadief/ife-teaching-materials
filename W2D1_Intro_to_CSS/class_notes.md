Hey everyone!

[Here's](https://www.youtube.com/watch?v=GPhyp7dgJsE) a link to today's lecture.

Great work this evening, and welcome to the world of CSS! Today we focused on color and font styling. Thursday's class we will start on the layout part!

#### The `<link>` Tag

The `<link>` tag tells our HTML "Hey, use this CSS file to style!"

This goes in the `<head>` section of our html page and points at the CSS file we want to use:

```html
<link rel="stylesheet" type="text/css" href="./style.css" />
```

#### Selectors

Here are the ways we looked at 'selecting' elements on our html page to style.

**_Tags_**

```css
/* Will be applied to all `<h1>` */
h1 {
  color: green;
}
```

**_Nested Selectors_**

```css
header h1 {
  color: tomato;
}
```

**_Classes_**

```css
.highlight {
  color: seagreen;
}
```

**_Classes_**

```css
.highlight {
  color: seagreen;
}
```

**_IDs_**

```css
#special {
  background-color: #000000;
}
```

####Specificity

In CSS we want to be as specific as possible so that our elements look the way we expect them to in browser.

- In order of priority:

  - Inline
  - ID
  - Class
  - Tag

#### Resources

**_Embedding custom fonts_**

- https://fonts.google.com

```html
<head>
  <link
    href="https://fonts.googleapis.com/css?family=Roboto+Mono"
    rel="stylesheet"
  />
</head>
```

```css
/* applying font to all <body> elements*/
body {
  font-family: "Roboto Mono", monospace;
}
```

**_Colors_**

- https://developer.mozilla.org/en-US/docs/Web/CSS/color_value

**_Box Model_**

- https://medium.freecodecamp.org/css-box-model-explained-by-living-in-a-boring-suburban-neighborhood-9a9e692773c1

**_Ipsums_** (_for when you want content to be created for you_)

- https://meettheipsums.com/

On Thursday we start learning about Flexbox! [Here's](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) a link to get you started on reading up on it.
