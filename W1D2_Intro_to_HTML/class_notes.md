Hey everyone! Thanks for another great class - your wireframes are looking fab!

[Here's](https://youtu.be/QL7STO_O8Vw) a link to today's lecture.

Here's today's notes and examples of the code we created in lecture.
Please feel free to reach out if you have any questions.

#### W1D2

Today we learned about HTML and what it does. Html has little to do with how our webpage actually _looks_, but it adds **context** to our **content**. The fun styley bit comes next week :grinning:

#### Atom

Atom is a text editor for our code! Here's some handy tips for using Atom:

- If there is a blue dot on your file tab then it means it hasn't been saved with your latest changes
- Some handy keyboard shortcuts:
  - Command + C - Copy
  - Command + V - Paste
  - Command + S - Save
  - Command + D - Select everything with the same text that I have selected
- Some useful packages to install to help make your life easier
  - atom-prettier _auto indents your code for you_
  - autoclose-html _closes your html tags automatically_

-To open you html file in your browser, click the bottom left button in Atom which is your filepath and paste it in the URL bar in your browser.

#### Web Page vs Web App

- A Web Page is purely informational and is static
- A Web App is interactive and dynamic

#### HTML tags

```
  <p> I'm a paragraph! </p>
```

Most HTML tags have:

- An opening tags
- Some content
- A closing tag

#### HTML Text Tags

These are a few of the common HTML tags that we use to wrap text in:

```
 <h1></h1
 <h7></h7>
 <p></p>
 <strong></strong>
 <em></em>
```

#### Nested tags

We can also next HTML tags together:

```
<div>
  <h3>My Awesome Webpage</h3>
</div>

```

Here the div is the parent and h3 is the child.

#### Semantic tags

Good HTML should tell a story and convey meaning. `<div>` tags are fairly generic, and if you have a tag that better explains what you are using it for - then you should use it over a div.

Some examples of semantic tags are:

```
<header>
<main>
<section>
<article>
<aside>
<footer>
<main>
```

[Here](https://developer.mozilla.org/en-US/docs/Glossary/Semantics) is a great resource for learning about HTML tags and semantic tags

#### Boilerplate

This is starter code for our web pages! We re-use this so we don't have to write the same thing over and over again.

```
<!DOCTYPE html>
<html>
  <head>
   	 <title>My Awesome Web Page</title>
  </head>
  <body>
  	<!-- Content goes here -->
  </body>
</html>

```

- `<!DOCTYPE html>` declaration defines this document to be HTML5
- `<html>` element is the root element of an HTML page
- `<head>` element contains information about the document and is used to link other files to your index.html
- `<title>` element specifies a title for the document
- `<body>` element contains the visible page content

#### Live Code

Here is the code that we wrote for the wireframe in class:

```
<!DOCTYPE html>
<html>
  <head>
    <title>My Awesome Resume Page</title>
  </head>

  <body>
    <header>
      <nav>
        <li>Link 1</li>
        <li>Link 2</li>
        <li>Link 3</li>
        <li>Link 4</li>
      </nav>
      <h4>Firstname Lastname</h4>
      <h7>Occupation</h7> <button>Button</button>
      <article>Image Here</article>
    </header>
    <main>
      <h6>About</h6>
      <p>PARAGRAPH ABOUT ME</p>
    </main>
  </body>
</html>
```

#### Remember to always indent! (or make your text editor do it for you)
