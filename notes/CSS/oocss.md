## OO-CSS (Object Oriented CSS)

Object Oriented CSS is a methodology that is focused on writing styles that are fast, maintable, predictable, and standards-based.

In OO-CSS, an "object" is a repeating visual pattern that can be abstracting into individual snippets or modules through a combination of HTML, CSS, and possibly JavaScript if necessary. An example would be the Google card design used in Google Now, tweets on Twitter, or posts on Facebook. Each have a distinct style that is repeated and recognizable. There may be slight variations in size based on content, but the majority of the styles remain the same. If each Google card had a `.card` class that represented that "object", a developer could use the `.card` class on another element with the confidence of knowing how that element is going to look and behaviour at different screen sizes, resolutions, etc.

## Principles

### Seperate Structure & Skin

**BAD**
<prism language='css'>
  img {

  }
</prism>

**GOOD**
<prism language='html'>
  <img class="image" />
</prism>

This principle means using classes to name objects as opposed to relying on HTML semantics. The "skin" represents the repeatitive visual styles that will be used on those objects and the "structure" is the HTML element that the skin is used on.

### Seperate Container & Content

<prism language='css'>
  .object h2 {

  }
</prism>

<!-- <prism language='html'>
  <h2 class="category"></h2>
</prism> -->

This principle means that an object should look the same no matter where it is used.