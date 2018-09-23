# HTML Style Guide
A style guide for writing consistent HTML code.

Based on and inspired by the following style guides:
- [Code Gudie by @mdo](http://codeguide.co/)
- [W3Schools HTML5 Style Guide](https://www.w3schools.com/html/html5_syntax.asp)
- [Google HTML/CSS Style Guide](https://google.github.io/styleguide/htmlcssguide.html)

## Capitalisation
Always use lowercase for:
- Element names
- Attributes
- Attribute values

## Indentation and blank lines
Indent by 2 spaces.

`<html>`, `<head>`, and `<body>` do not need to be indented to avoid over-indentation of the document.

Any child elements of `<head>` and `<body>` should be indented, as should nested elements.

Use blank lines to separate large or logical code blocks, but do not add unnecessary blank lines.
```html
<!DOCTYPE html>
<html>
<head>
  <title>This is a page title</title>
</head>

<body>
  <p>Hello, world!</p>
  <ul>
    <li>Item 1</li>
    <li>Item 2</li>
  </ul>
</body>
</html>
```
## Attributes
Attribute values should always be quoted using double quotation marks.

In most cases, multiple attribute values should be separated by a single space.
```html
<a class="button sign-in">Sign in here</a>
```
Use the following order for HTML attributes:
- `class`
- `id`, `name`
- `data-*`
- `src`, `for`, `type`, `href`, `value`
- `title`, `alt`
- `role`, `aria-*`

## Images
Always provide an `alt` attribute for images to improve accessibility.
```html
<img src="images/tree.png" alt="A picture of an oak tree">
```

## Closing elements
All HTML elements should include a closing tag.
```html
<p>This is some paragraph text</p>
```

## Void Elements
Don't include a trailing slash in void, or self-closing, elements.
```html
<img src="images/sunset.png" alt="An image of a sunset">
```
## HTML Doctype
Always declare the HTML doctype as the first line in a document.
```html
<!DOCTYPE html>
```
## `<html>`, `<head>`, and ,`<body>`
The `<html>`, `<head>`, and ,`<body>` elements should not be omitted from a HTML document.

## Language attribute
Specify a language attribute on the root `<html>` element, detailing the language of the document, to assist screen reading technology.
```html
<html lang="en">
```
## Character encoding
To ensure proper rendering of content specify the character encoding as high as possible in the document `<head>`.

Use UTF-8 encoding.
```html
<meta charset="UTF-8">
```
## Internet Explorer Compatability
Use the `X-UA-Compatible` meta tag to specify which version of Internet Explorer a page should be rendered as.

Unless it is required otherwise, the `IE=edge` option should be used to display content in the highest available mode.

The tag should be placed as high as possible in the document `<head>`.
```html
<meta http-equiv="X-UA-Compatible" content="IE=edge">
```
## Viewport Setting
A `<meta>` viewport element should be used to provide instructions to a browser on how to control a page's dimensions and scaling.

Use `width=device-width` to set the width of the page to follow the screen width of the device.

Use `initial-scale=1.0` to set the initial zoom level of the page when it is first loaded.
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
## Linking to CSS and JavaScript files
As HTML5 uses `text/css` and `text/javascript` as default values there is no need to specify the `type` attribute when linking to style sheets and script files.
```html
<link rel="stylesheet" media="screen" href="styles.css">
<script src="script.js"></script>
```
