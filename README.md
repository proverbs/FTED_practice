# FTED_practice

## HTML

### Resources:
- https://learn.shayhowe.com/html-css/building-your-first-web-page/
- http://htmldog.com/guides/html/

### Terms
- elements: `<a>`
- tags: 
    - opening tags, closing tags: `<a>...</a>`. 
    - self-closing tags: `<img>`, `<meta>`.
- attributes: defined within the opening tags. `<a href="http://shayhowe.com/">Shay Howe</a>`.

### Typical Structure
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>Hello World</title>
  </head>
  <body>
    <h1>Hello World</h1>
    <p>This is a web page.</p>
  </body>
</html>

```

### Code Validator
- http://validator.w3.org/

### Elements
- containers: `<div>`(block-level) and `<span>`(inline-level)
- headings: `<h1>` - `<h6>`
- paragraphs: `<p>`
- bold texts with strong: `<strong>` and `<b>`
- italicize texts with emphasis: `<em>` and `<i>`

### Structural Elements(block-level)
- `<header>` 
- `<nav>`
- `<article>` 
- `<section>`
- `<aside>`
- `<footer> `

### Encoding Special Characters
- begin with an ampersand(&) and end with a semicolon(;)

### Hyperlinks
- anchor, `<a href="https://proverbs.github.io">Proverbs' Blog</a>`
- path can be either relative or absolute
- open in new window: `<a href="..." target="_blank">`
- link to parts of the same page: `<a href="#top">back to top</a>`
- email link with `mailto:`

## CSS

### Terms
- selectors: `p { ... }` for `<p>`.
- properties:

    ```css
    p {
    color: ...;
    font-size: ...;
    }
    ```
- values:
  
    ```css
    p {
    color: orange;
    font-size: 16px;
    }
    ```

### Selectors(different specificity from low to high)
- type selectors(point value of 0-0-1): `div { ... }`
- class selectors(point value of 0-1-0): `.awesome { ... }`, `<div class="awesome">...</div>`
- ID selectors(point value of 1-0-0): `#shayhowe { ... }`, `<div id="shayhowe">...</div>`
- combined selector: 
    - `.class_name p {...}` will select paragraphs in(no need to be directly in) elements with the class name of `class_name`. Explanation: p is the **key selector**, the others are **prequalifers**
    - `p.class_name {...}` will select paragraphs with the class name of `class_name`
- **specificity** 
    - only applies to elements directly selected, not apply to children elements
    - add specificity for combined selector
    - to avoid high specificity, selectors should be modular:

        ```html
        <a class="btn btn-danger">...</a>
        <a class="btn btn-success">...</a>
        ```

        ```css
        .btn {
        font-size: 16px;
        }
        .btn-danger {
        background: red;
        }
        .btn-success {
        background: green;
        }
        ```

### Reference CSS in HTML
```html
<head>
  <link rel="stylesheet" href="main.css">
</head>
```

### CSS Resets
Different web browsers render pages using different predefined styles, so we need to reset the styles for compatibility.
- [Eric Meyer’s reset](https://meyerweb.com/eric/tools/css/reset/)

### Cascade
- top style can be overwritten by bottom style

### CSS Colors
- keyword colors: black, gray, ...
- hexo values: `#000000` for black
- rgb values: `rgb(0, 0, 0)` for black
- rgba values: `rgba(0, 0, 0, .5)` for opaque black

### CSS Lengths
- absolute lengths
    - pixels: `font-size: 14px;`
- relative lengths
    - percentages: `width: 50%`
    - `width: 5em`, its length is calculated based on an element’s font size