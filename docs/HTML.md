## HTML

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