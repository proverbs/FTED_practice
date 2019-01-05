## Box Model

> Block-level elements occupy any available width, regardless of their content, and begin on a new line. Inline-level elements occupy only the width their content requires and line up on the same line, one after the other.
> Block-level elements are generally used for larger pieces of content, such as headings and structural elements. Inline-level elements are generally used for smaller pieces of content, such as a few words selected to be bold or italicized.

### Display
- `display: block;`
- `display: inline;`
- `display: inline-block;`: accepte all box model properties, but displayed inline
- `display: none;`: not displayed

### Box Model
**Every element on a page is a rectangular box.**
- from outside to inside: `margin`, `border`, `padding`, `hight/width`
    ```css
    div {
      border: 6px solid #949599;
      height: 100px;
      margin: 20px;
      padding: 20px;
      width: 400px;
    }    
    ```
- element's total height and width
    - height: margin-top + border-top + padding-top + height + padding-bottom + border-bottom + margin-bottom
    - width: margin-right + border-right + padding-right + width + padding-left + border-left + margin-left
- Width & Height
    - width: block-level: 100%; inline and inline-block: accommodate content
    - height: accommodate content
    - inline-level elements will not accept the width and height properties 
- Margin: **transparent**; top/bottom not accepted, margin accepted by inline elements
- Padding: **transparent**; **withint element**
- Border: width, style, color.
    - style: solid, double, dashed, dotted, and none.
        ```css
        div {
            border: 6px solid #949599;
        }
        ```
    - individual border sides: 
        ```css
        div {
            border-bottom: 6px solid #949599;
        }
        div {
            border-bottom-width: 12px;
        }
        ```
    - border-radius: round corner elements

### Box Sizing
- content box(default): `box-sizing: content-box;`, add outside the width and height
- border box: `box-sizing: border-box;`, add inside the width and height
- 