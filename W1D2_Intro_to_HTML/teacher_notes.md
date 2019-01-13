# Intro to Front End - Intro to HTML

**_Set up the Live Stream_**

### Front End Fundamentals

- How did you find Monday's work?

### Intro to HTML

- Has anyone used HTML before?
- Today is intro to HTML
- Does everyone have a wireframe from last class?
- By the end of today we’re going to be able to take your wireframes from last class and turn them into code
- We'll also talk about semantic tags and why they are important
- Indenting and why it's important

### Meet Atom, our code editor

- Does anyone have Atom installed?
- Get them to download from https://atom.io

- Tour of Atom
- Open up Atom
- Open up folder - this is project directory, this is my file

- Can anyone tell me what changes when I stop typing here?
- Shortcut to save is Command + S on a Mac or Ctrl + C

**_Packages_**

- These can make your life easier
- Prettier
- Auto close

### Web Pages

- Websites are static, whereas web apps are dynamic
- Regardless - both of these use HTML to create their structure

### Wire Frame

- Here’s a wireframe! What shape are we seeing a lot of?
- Each one of these is an HTML element.
- Today we’re not going to worry about making things look pretty or even good
- Gonna look like from 90's
- Today the only thing we’re dealing with is the content.

#### HTML

- What does HTML stand for?
- Hyper Text Markup Language
- What does that mean?
- Language that lets us display content on the internet
- Gives structure to your webpage.
- It can give **_context_** to your **_content_**

**_Metaphor_**

- I just got a new bed from Ikea
- HTML is like the bedframe.
- Mattress is the content - the bedding and the pillows are the styling.
- We’re not going to worry about those for now because those are the decorations.
- You have headboard, box frame, and foot

---

**_Live Code_**

Now we're going to see how this translates as HTML:

- Open up Atom
- Show HTML Skeleton
- We'll go through what each of these mean through the lecture
- We use this to build an HTML page

```html
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

---

#### The HTML Tag

- An HTML tag is composed of three main parts

  - An Opening Tag
  - Some content
  - A closing tag

- Most HTML tags follow this pattern
- Tons of different HTML tags
- Don't worry about memorizing them all

---

**_Live Code_**

- Type out this code in Atom:
- Open up in browser

```html
<p>I’m an HTML tag</p>
```

#### Tags for Text

- Several HTML tags that we can use to wrap text in.
- Browser assigns default stylings to these
- We can override using CSS

---

**_Live Code_**

- Show tag and point out default styling with Dev Tools
- Show what would happen if you missed a closing tag.
- Add each of the following to the HTML skeleton:
- Explain Lorem Ipsum

```html
<h1>Title</h1>
<p>
  Lick the curtain just to be annoying chirp at birds shake treat bag fooled
  again thinking the dog likes me, leave fur on owners clothes flex claws on the
  human's belly and purr like a lawnmower. Pee in human's bed until he cleans
  the litter box have secret plans. Burrow under covers my water bowl is clean
  and freshly replenished,
</p>
<strong>Strong</strong> <em>Em</em>
```

---

#### Nesting Tags

- We can also nest tags inside each other.
- Indentation!
- Close child tags before you close parent tags
- We refer to relationships between elements (parents, children, siblings).
- You can nest as many elements as you would like.

---

**_Live Code_**

- Nest your `<h1>` from the previous example in a `<div>`
- A `<div>` is a container element
- Wrap the `<p>` tag inside

---

#### Semantic tags

- Div from the code is an example of 'div soup'
- Most tags in markup in most modern webpages are `<div>` tags

- Great markup conveys meaning;
- It tells the story about what's inside.
- Markup should make the developer's life easier by aiding readability and reducing the amount of work required to understand the code.
- The way to fix that is to use semantic tags

#### Div Tags

- Semantic tags describe their purpose
- While divs are useful for generic containers
- If you have a semantic tag that serves your purpose you _should_ use it

This code is contrasted with the next slide

- What is the purpose of this first div?
- What about the next one?

```html
<div><h1>My Awesome Webpage</h1></div>
<div>
  <div>
    <h3>Article Title</h3>
    <p>I’m an article</p>
  </div>
</div>
```

### Semantic Tags

- This is an example of some semantic tags in use.
- The header tells us this is a header
- Main usually encompasses the main section of your page
- Article tells us this is a container within main
- How is this different from the previous slide?
- Does anyone want to take a guess at the parent/child relationships in this code?

```html
<header><h1>My Awesome Webpage</h1></header>
<main>
  <article>
    <h3>Article Title</h3>
    <p>I’m an article</p>
  </article>
</main>
```

#### HTML Skeleton

- Boilerplate is what we call starter code
- There are some things that will _always_ be in an HTML page
- So let's use pre-written code

```html
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

#### HTML Skeleton Contd...

- Different components of an HTML Skeleton
- The `<!DOCTYPE html>` declaration defines this document to be HTML5
- The `<html>` element is the root element of an HTML page
- The `<head>` element contains meta information about the document
- The `<title>` element specifies a title for the document
- The `<body>` element contains the visible page content

- Indentation indentation indentation
- Head and Header are easy to mix up

- Head acts like the brain of the website, your links and important data go here
- Header is a tag name

---

**_Live Code_**

Go back to HTML live code and explain each element

---

#### Wireframes to HTML

- Remember the wireframes you made?
- Wireframes are simple black and white layouts that outline the specific size and placement of page elements, like a blueprint for your webpage
- These are a basis for the HTML created

#### Wireframes to HTML Contd...

- Look at this slide and then let's create an HTML file using semantic tags
- Start with Boilerplate
- I'm going to make some syntax errors. See if you can spot them!

---

**_Live Code_**

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My Awesome Web Page</title>
  </head>
  <body>
    <header>
      <nav>
        <li>Link 1</li>
        <li>Link 2</li>
        <li>Link 3</li>
        <li>Link 4</li>
      </nav>
      <h4>FirstName LastName</h4>
      <h7>Occupation</h7> <button>Button</button> <img />
    </header>
    <article>
      <h2>About</h2>
      <p>
        Lick the curtain just to be annoying chirp at birds shake treat bag
        fooled again thinking the dog likes me, leave fur on owners clothes flex
        claws on the human's belly and purr like a lawnmower. Pee in human's bed
        until he cleans the litter box have secret plans. Burrow under covers my
        water bowl is clean and freshly replenished,
      </p>
    </article>
  </body>
</html>
```
