## The DOM

The DOM, which stands for Document Object Model, is a representation of how the browser how constructed the "tree" of the HTML elements of the web page upon load.

If the DOM is changed via JS, the changes are reflected instantly without page refresh. This includes new and removed elements, attributes, and styles, which is frequently used for such things as updating the DOM to reflect new data and notifying the user of relevant information, such as how GMail notifies the user that they have a new email without having to refresh the page.

## Elements

~~~html
<tagname> content </tagname>
~~~

* It is a convention to use lowercase letters when writing tagnames

### Head
~~~html
<head>
  <title> Meowcakes! </title>
</head>
~~~

The HTML <head> element represents a collection of metadata about the document, including links to or definitions of scripts and style sheets.

### Headings
```html
  <h1> Meowcakes! </h1>
```

Heading elements implement six levels of document headings, `<h1>` is the most important and `<h6>` is the least. A heading element briefly describes the topic of the section it introduces. Heading information may be used by user agents, for example, to construct a table of contents for a document automatically.

### Content Tags

```html
<ul>
```

Unordered list (list with bullets)

```html
<ol>
```
Ordered list (list with numbers)

```html
<li>
```
List item ( used within ul and ol elements )

```html
<em>
```
Renders as emphasised text

```html
<strong>
```
Defines important text

```html
<dfn>
```
Defines a definition term

```html
<code>
```
Defines a piece of computer code

```html
<samp>
```
Defines sample output from a computer program

```html
<kbd>
```
Defines keyboard input

```html
<var>
```
Defines a variable

```html
<img>
```
Used to insert image

```html
<img src="path/to/file.fileextension"/>
```

```html
<a href="url">  Link Text </a>
```
Used to insert a clickable link
* If you would like the link to open up a new tab, you can add ``target='_blank'`` inside of the `<a>` tag as so: ``<a src='google.com' target='_blank'>Link Text</a>``
* ``<div>``, ``<section>``, ``<article>``, ``<span>``
```<div> <!-- content --> </div>```
```<section> <!-- content --> </section>```
```<span> <!-- content --> </section>```

* Divs and sections are used to contain other elements. They are used for this because they do not have any default styles.

* Spans have the same properties as divs, except they are inline elements, while divs and sections are block elements the page does not load without it's styles

* ``<link>`` Primarily used to include a CSS file
```
<link rel="stylesheet" href="path/to/css/file"/>
```
* CSS files are included within the <head> section of the HTML document so that

* ``<script>`` Used to either include a JS file or insert JS code directly into the html document
```
<script src="path/to/js/file"></script>
```
* JS files are commonly included at the bottom of the ``<body>`` section of the HTML document so that the page can render and user can begin interacting with the webpage before the JS files need to be downloaded.

#### Classes and Ids
```html
<tagname class="classname"> content </tagname>
<tagname id="idname"> content </tagname>
```
Classes and ids are attributes of an HTML element. They are used to differentiate elements from each other, which comes in very handy when defining styles in CSS and behaviours in JavaScript. It is recommended to use classes for defining styles in CSS and ids for referencing that element in JavaScript.
********
#### Image Extensions
Common image extensions are .jpg, .png, .tiff, and .gif. The most popular being:

1. **jpeg** The JPEG compression algorithm is at its best on photographs and paintings of realistic scenes with smooth variations of tone and color. For web usage, where the amount of data used for an image is important, JPEG is very popular. JPEG/Exif is also the most common format saved by digital cameras.

2. **gif** GIFs are suitable for sharp-edged line art (such as logos) with a limited number of colors. This takes advantage of the format's lossless compression, which favors flat areas of uniform color with well defined edges. They can be used to store low-color sprite data for games. They can be used for small animations and low-resolution film clips. Since a single GIF image palette is limited to 256 colors, it is not usually used as a format for digital photography. Digital photographers use image file formats capable of reproducing a greater range of colors, such as TIFF, RAW or JPEG.

3.  **png** Similar to jpegs, but are larger files and allow for alpha transparency

## Best Practices
* Keep nested elements indented one tab in comparison to their parent element
* Build as much of the HTML for a page as possible before attempting to style it.
