## W3D2 Responsive Design & Deployment

Hey everyone! Awesome work tonight - we're officially halfway through the program! This concludes our HTML and CSS portion of the course, and next week we start on Javascript.

### Review

Today we did a quick review of the Advanced CSS learned on Monday:

- Advanced Selectors
  - Stacking `.child-a, .child-b`
  - Adjacent `p + p`
  - General Sibling `div ~ div`
- Pseudo-Selectors
  - Styles in Specific state `.child:hover`
- Pseudo-Elements
  - Style parts of the element itself `.child::selection`
- Transition Shortcut
  - Animate changes when triggered by an event `transition: background-color 2s ease-in-out`

### Media Queries

Media Queries are how we make our webpages responsive to different screen sizes - especially on mobile.

We use Breakpoints to set the point at which our responsive styles get triggered.

- Large Screens / Desktop
  - Any screen over 1024px wide (including a tablet being viewed in landscape)
- Medium Screens / Tablets
  - Any screen between 768px and 1024px
- Small Screens or Phones
  - Lots of variety in phone size but the largest size is 480px

Media Query

```
    @media screen and (max-width: 660px) {
        div {
          font-size:: 24px
        }
    }
```

Anything you place in this media query will override any default styles and apply it to your HTML when it matches the specified width.

[Jen Simmons](http://jensimmons.com/) Has some great responsive styles and some awesome front-end youtube videos.

### Parallax

Parallax is a nice image effect where text scrolls on top while the image stays put.

We can achieve this in three steps:

1. Set Background Image

- Use `background: url('./image')` where the './image' references the url or filepath to the image you want to use.

2. Set Background Size

- Set the size of the background image with `background-size: cover;`. For Parallax use 'cover' which makes the image as large as possible without stretching it. CSS will crop the images width or height to eliminate any empty space.
- 'contain' scales the image as large as possible without stretching or cropping it.

3. Set Background Attachment

- `background-attachment: fixed` This only works when a background image is specified. It determines if the image stays in place or scrolls with the content.

### Deployment

We deployed! Yay!

In order to deploy your site to getforge.io:

1. Sign up for https://getforge.com/
2. Create site on GetForge
3. Zip your project folder on your computer
4. Upload the zip file
5. Navigate to your URL
   ([Echo's page](echo.getforge.io))

Also [here's](https://css-tricks.com/snippets/css/keyframe-animation-syntax/) a final link to some stretch reading on more CSS Animation
