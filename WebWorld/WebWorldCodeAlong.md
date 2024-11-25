# Code-Along: Web Wave
Follow these instructions to build a hackathon website of your own 🕶

## Getting Started
Get started by grabbing some starter code on Glitch.

1. [Click here to open and remix the starter project](https://glitch.com/edit/#!/remix/web-world-start)
1. Open the **index.html** from the file selector on the left
1. Open the preview pane from the bottom menu

That's it! You should be all set, and ready to code.

## Looking at the HTML
Make sure the **index.html** file is selected on the left to view the HTML code. Notice how the code in the HTML creates the text on the website. Everything in HTML goes between _tags_, which tell the website what type of element to display. There are a lot of tags right now, but the important stuff goes between the `<body>` and `</body>` tags. For example, the text between the `<h1>` and `</h1>` tags becomes a large header.

The first thing to do is update the header text with your website topic! Unless you want to make a website about your grandma, which is totally fine.

Update the code in the HTML section, _between_ the `<h1>` and `</h1>` tags. It should look something like this:

```html
<h1>A Website About My Grandma</h1>
```

The area on the right should automatically update with the new text. You're officially a web developer!

## Adding a Welcome Paragraph
Now it's time to add a totally new element. The **paragraph** element is used to display normal text on a webpage. Its tags are `<p>` and `</p>`, with text content between.

1. Make a new line underneath the `<h1></h1>`
    - Still within the `<body>` and `</body>`
1. Add a `<p>` opening tag on the new line
1. Enter some text that will be displayed
    - Ex: "My grandma was a really cool lady."
1. At the end of the line, add a `</p>` to close the paragraph element
1. Run the project, and verify that the message appears on the website!

The code should look something like this:

```html
<p>My grandma was a really cool lady.</p>
```

## Adding a Cool Image
Almost every website has at least one image, and yours can too! We'll start by adding the code for a new element, and then we'll find a picture URL we can use.

### The HTML
The image can be added using the `<img>` element. Note that this element is special; it only has an opening tag, no closing tag.

1. Make a new line under the `<p></p>`
2. Add a new element: `<img >`
3. After the `img`, before the `>`, type in `src=""`
   
Make sure it looks exactly like this:

```html
<img src="">
```

### Finding a Picture
If you want to use a picture of your own, you can find a URL online!

1. Open a new tab, but make sure to keep the Glitch open too
1. In the new tab, go to [google images](https://google.com/images/)
2. Search for an image you would like on your webpage (e.g., _my grandma_)
3. Click on the image, and make sure it fully loads on the right side of the page
4. Right click the picture, and choose "Copy image address" OR "Copy image link"
    - This will depend on your browser
5. Open the code editor again
6. Paste the URL right in between `"` and `"`
7. 
The code should look the same - just update what's within the `"` and `"` after `src=` in the `<img >` tag!

```html
<img src="https://example.com/my-cool-img.jpg">
```

### Resizing
The image might be gigantic - that's alright! There are several ways to update the size of an image in HTML.

1. Find the `<img>` element in the code
1. After the `src=""`, but _before_ the `>`, make a new space
1. Add `width="200px"`
    - This sets the _width_ of the image to _200 pixels_
1. Run the project to see the image shrink or grow!
    - Feel free to update the number of pixels for different sizes

The code should look something like this:

```html
<img src="assets/purple.jpeg" width="200px">
```

## Adding Another Page
The homepage for the website is looking pretty good, but we want to do more! Creating multiple HTML pages is a great way to organize all the information on a site. This is possible with a new **.html** file, and the `<a></a>` anchor element.

### Creating the New File
Start by creating a whole new **.html** file for a new webpage.

1. In the **Files** area, click the "New file" button  
2. Enter a name for the file ending with **.html** (e.g., **grandpa.html**)
3. Click the "Add This File 🌱" to create it
4. The new file should open automatically in the Code Editor
5. Copy the basic HTML boiler-plate from the **index.html** file
6. Replace the `<h1></h1>` text with something like "My Grandpa is Also Cool"
7. Replace the `img` source with a new picture URL
8. Add a `<p></p>` with a quick blurb about something like your grandpa

The **grandpa.html** file should contain text that looks something like this:

```html
<html>
  <head>
    <link href="extras/fonts.css" rel="stylesheet" />
    <link href="style.css" rel="stylesheet" />
    <script src="script.js" defer></script>
  </head>
  <body>
    <h1>My Grandpa is also cool</h1>
    <p>I love my grandpa</p>
    <img src="https://example.com/my-grandpa.png">
  </body>
</html>

```

### Linking the New File
The new page has some good content, but there's no easy way to see it right now! We can use the `<a></a>` anchor element to create a _hyperlink_ from the homepage to the new page. An `<a></a>` element looks like this:

```html
<a href="link.html">Display Text</a>
```

- The text within the `href="` and `"` specifies the destination of the link
- The text within the `<a>` and `</a>` specifies the text that will appear for the link

Follow these steps to add a link to the **grandpa.html** file:

1. From the **Files** area, click the **index.html** file to open it
1. After the `<img>` element, make a new line
1. Add an `<h2></h2>` element that says "Navigation"
1. Make another new line under the `<h2></h2>`
1. There, create an `<a></a>` element
1. Set the `href` to be `grandpa.html` (between `"` and `"`)
1. Set the text to be "My Grandpa"
1. Run the project, click the link, and verify that the Grandpa page appears!

The additional code in the **index.html** file should look something like this:

```html
<h2>Navigation</h2>
<a href="grandpa.html">My Grandpa</a>
```

### Linking Back
Now it's possible to view the Grandpa page, but there's no way to get back home! We need another `<a></a>` element in the **grandpa.html** file. We can also add a link to an _external_ website!

1. From the **Files** area, click the **grandpa.html** file to open it
1. After the `<p></p>` element, make a new line
1. There, create an `<a></a>` element
1. Set the `href` to be `index.html` (between `"` and `"`)
1. Set the text to be "Home"
1. Make another new line after that
1. Create another `<a></a>` element
1. Set the `href` to be `https://en.wikipedia.org/wiki/Grandparent` (between `"` and `"`)
1. Set the text to be "More"
1. Run the project, click the "Grandpa" link, and verify that it is possible to navigate back home!

The additional code in the **grandpa.html** file should look something like this:

```html
<a href="index.html">Home</a>
<a href="https://en.wikipedia.org/wiki/Grandparent">More</a>
```

## Changing the Background Color with CSS
Now the content of the website is looking pretty good, but it's not very stylish. One way to make the website look more fun and exciting is to use CSS! HTML is like the skeleton of a webpage, just the structure, and CSS is like the clothes that it wears, giving it style.

From the **Files** area, open the **style.css** file by clicking on it. Take a look at the code so far. Try to figure out how to change the background color from `white` to another color, like `pink`!

The code should look something like this:

```css
body {
    background: pink;
}
```

Run the project, and see the background change!

## Changing More with CSS
CSS can change almost anything on a website. For this activity, update the text color, size, and font! All changes should take place in the **style.css** file.

### Updating the Text Color
Follow these instructions to change the text color on your website.

1. Find the line where the `background` color is set
1. Make a new line underneath that line (above the `}`)
1. Type in `color`, followed by a colon (`:`)
1. Make a space, and type in a new color (like `purple`) followed by a semi-colon (`;`)

Run the project, and verify that the text color changes!

Note that every CSS _property_ follows the same structure:

- Property name (e.g., `color`)
- Colon (`:`)
- Property value (e.g., `purple`)
- Semi-colon (`;`)

### Updating Font and Size
Next, update the font and size of the text by following the instructions below.

1. Make a new line under the `color` line (still above `}`)
2. Set a new property `font-family` to a value of `"Oswald"`
    - property name, colon, property value, semi-colon
    - This name can also be anything from the **extras/fonts.txt** file!
3. Make another new line, still above `}`
4. Set another new property `font-size` to a value of `18px`
    - property name, colon, property value, semi-colon

Run the project, and verify that the text changes font and size! Feel free to try changing the numbers or the font to see what works.

The code should look something like this:

```css
body {
  background: pink;
  color: purple;
  font-family: "Oswald";
  font-size: 18px;
}
```

## Using Custom Colors
Some basic colors are built into the web (like **pink** and **purple**), but it is also possible to use custom colors! Each color can be represented as a _hexidecimal color code_, which is a hashtag (`#`) followed by six alphanumeric characters. The easiest way to find a specific color is to use a color picker.

1. Open a new tab, and [google "color picker"](https://www.google.com/search?q=color+picker)
1. Drag the circles around to find a good color
2. Copy the text from the "HEX" section (starting with a **#**)
3. Go to the **style.css** file
5. Paste the hex code in place of one of the colors, or both!

The CSS code should look something like this:

```css
body {
    background: #ffbdbd;
    color: #bf3636;
    font-family: "Oswald";
    font-size: 18px;
}
```

## Adding Interactivity with JavaScript
JavaScript is a perfect way to create more powerful websites that respond to user input and do interesting things. The Glitch project already has some JavaScript code in it, within the **script.js** file!

```js
function displayMessage() {
  alert("Welcome to JavaScript World!");
}
```

This code sets up a _function_ named `displayMessage`. We can _call_ the `displayMessage` function to run the code in its body. It will display a message box.

1. Open the **index.html** file for editing
2. At the bottom of the rest of the content, add a new HTML element: a `<button></button>`
3. Within the opening `<button>` tag, add an `onclick` attribute
   - This is just like the `src` attribute on the `<img src="">` element!
   - Attribute name, equals sign, and double quotes
4. Set the value of the `onclick` to be `displayMessage()`
    - This should go right between the double quotes
5. Finally, in between the opening and closing `<button></button>` tags, add text that says "Click Me"

The added code should look something like this:

```html
<button onclick="displayMessage()">Click Me</button>
```

Reload the page, click the button, and see what happens - it should display a message!

### Challenge: Displaying a Different Message
If you wanted to display something different, you could update the code in the **script.js** file.

## Conclusion
Congratulations, you've successfully built your own website! It may seem simple so far, but these concepts form the basis of everything on the web. You can continue to fill out this website, or start a totally new site, and build from there. Make sure to check out the many resources available for further learning and exploration!

[Click here to go back home.](Home.md)
