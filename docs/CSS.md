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