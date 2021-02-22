[HOME](https://mousasbbah.github.io/reading-notes/)

# Layout in CSS

## Controlling the Position of Elements
CSS has the following **positioning schemes** that allow you to control
the layout of a page: normal flow, relative positioning, and absolute
positioning. You specify the positioning scheme using the position
property in CSS. You can also float elements using the float property.

* **Normal Flow**

    In normal flow, each block-level
element sits on top of the next
one. Since this is the default
way in which browsers treat
HTML elements, you do not
need a CSS property to indicate
that elements should appear
in normal flow, but the syntax
would be:
**`position: static;`**

* **Relative Positioning**

  Relative positioning moves an
element in relation to where it
would have been in normal flow.
For example, you can move it 10
pixels lower than it would have
been in normal flow or 20% to
the right.the syntax
would be:
**`position: relative;`**

* **Absolute Positioning**

  When the position property
is given a value of absolute,
the box is taken out of normal
flow and no longer affects the
position of other elements on
the page. (They act like it is not
there.)
The box offset properties (top
or bottom and left or right)
specify where the element
should appear in relation to its
containing element.


*  **Fixed Positioning**

    Fixed positioning is a type
of absolute positioning that
requires the position property
to have a value of fixed.
It positions the element in
relation to the browser window.


   Therefore, when a user scrolls
down the page, it stays in the
exact same place. It is a good
idea to try this example in your
browser to see the effect.

* **Floating Elements**

  The **`float`** property allows you
to take an element in normal
flow and place it as far to the
left or right of the containing
element as possible.
Anything else that sits inside
the containing element will
flow around the element that is
floated.

### Screen Sizes 

  **Different visitors to your site will have different sized screens that show
different amounts of information, so your design needs to be able to
work on a range of different sized screens.**

### Screen Resolution
  **Resolution refers to the number of dots a screen shows per inch. Some devices have a higher resolution than desktop computers and most
operating systems allow users to adjust the resolution of their screens.**

### Page Sizes

  **Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide**

### Fixed Width Layouts
Fixed width layout
designs do not
change size as the
user increases
or decreases
the size of their
browser window.
Measurements tend
to be given in pixels.

### Liquid Layouts

  Liquid layout designs
stretch and contract
as the user increases
or decreases the
size of their browser
window. They tend to
use percentages.

### Layout Grids
Composition in any visual art (such as design, painting, or photography)
is the placement or arrangement of visual elements — how they are
organized on a page. Many designers use a grid structure to help them
position items on a page, and the same is true for web designers.

### Possible Layouts: **960** Pixel wide **12** Column Grid

<br>

![px](/image/px.bmp)

### CSS Frameworks
CSS frameworks aim to make your life easier by providing the code for
common tasks, such as creating layout grids, styling forms, creating
printer-friendly versions of pages and so on. You can include the CSS
framework code in your projects rather than writing the CSS from scratch.

[HOME](https://mousasbbah.github.io/reading-notes/)