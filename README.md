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

### Selectors
- type selectors: `div { ... }`
- class selectors: `.awesome { ... }`, `<div class="awesome">...</div>`
- ID selectors: `#shayhowe { ... }`, `<div id="shayhowe">...</div>`


### Reference CSS in HTML
```html
<head>
  <link rel="stylesheet" href="main.css">
</head>
```

### CSS Resets
Different web browsers render pages using different predefined styles, so we need to reset the styles for compatibility.
- [Eric Meyer’s reset](https://meyerweb.com/eric/tools/css/reset/)

