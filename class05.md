# HTML 

## Images 


### **Adding Images**

```html 
<img src=""  alt=""  title="" />
```
To add an image into the page
you need to use an `<img>`
element. This is an empty
element (which means there is
no closing tag). It must carry the
following two attributes:


**`src`**

This tells the browser where
it can find the image file. This
will usually be a relative URL
pointing to an image on your
own site.

**`alt`**
---
This provides a text description
of the image which describes the
image if you cannot see it.

**`title`**

You can also use the title
attribute with the `<img>` element
to provide additional information
about the image. Most browsers
will display the content of this
attribute in a tooltip when the
user hovers over the image.

### **Height & Width of Images**


You will also often see an `<img>`
element use two other attributes
that specify its size:

**`height`**

This specifies the height of the
image in pixels.

**`width`**

This specifies the width of the
image in pixels.

### HTML 5: Figure and Figure Caption

**`<figure>`**

Images often come with
captions. HTML5 has introduced
a new **`<figure>`** element to
contain images and their caption
so that the two are associated.
You can have more than one
image inside the **`<figure>`**
element as long as they all share
the same caption.

**`<figcaption>`**

The **`<figcaption>`** element has
been added to HTML5 in order
to allow web page authors to add
a caption to an image.

## Color 

The color property allows you
to specify the color of text inside
an element. You can specify any
color in CSS in one of three ways:
   * **RGB values**

      These express colors in terms
of how much red, green and
blue are used to make it up. For
example: `rgb(100,100,90)`
   * **Hex Codes**
   
      These are six-digit codes that
represent the amount of red,
green and blue in a color,
preceded by a pound or hash `#`
sign. For example: `#ee3e80` 
   * Color Names

      There are 147 predefined color
names that are recognized
by browsers. For example:
`DarkCyan`

### CSS3 OPACITY
CSS3 introduces the `opacity`
property which allows you to
specify the opacity of an element
and any of its child elements.
The value is a number between
0.0 and 1.0 (so a value of 0.5
is 50% opacity and 0.15 is 15%
opacity).


The CSS3 `rgba` property allows
you to specify a color, just like
you would with an RGB value,
but adds a fourth value to
indicate opacity. This value is
known as an alpha value and is
a number between 0.0 and 1.0
(so a value of 0.5 is 50% opacity
and 0.15 is 15% opacity). The
rgba value will only affect the
element on which it is applied
(not child elements).

### CSS3 HSL & HSLA

The `hsl` color property has
been introduced in CSS3 as an
alternative way to specify colors.
The value of the property starts
with the letters hsl, followed
by individual values inside
parentheses for:

**hue**

This is expressed as an angle
(between 0 and 360 degrees).

**saturation**

This is expressed as a
percentage.

**lightness**

This is expressed as a
percentage with 0% being white,
50% being normal, and 100%
being black.


The hsla color property allows
you to specify color properties
using hue, saturation, and
lightness as above, and adds a
fourth value which represents
transparency (just like the rgba
property). The a stands for:

**alpha**

This is expressed as a
number between 0 and 1.0.
For example, 0.5 represents
50% transparency, and 0.75
represents 75% transparency.


##  Text

### Specifying Typefaces

`font-family`

The font-family property
allows you to specify the
typeface that should be used for
any text inside the element(s) to
which a CSS rule applies.

The value of this property is the
name of the typeface you want
to use.

The people who are visiting
your site need the typeface you
have specified installed on their
computer in order for it to be
displayed.

### Size of Type

`font-size`

The font-size property enables
you to specify a size for the
font. There are several ways to
specify the size of a font. The
most common are:

* pixels
* percentages
* ems

**Units of Type Size**

![Default Size](/image/defaultSize.bmp) 

### Bold

The `font-weight` property
allows you to create bold text.
There are two values that this
property commonly takes:

* `normal`

  This causes text to appear at a
normal weight.
* `bold`

   This causes text to appear bold.

### Iticle

If you want to create italic text,
you can use the **`font-style`**
property. There are three values
this property can take:

* `normal`

  This causes text to appear in a
normal style (as opposed to italic
or oblique).

* `italic`

  This causes text to appear italic.
* `oblique`

  This causes text to appear
oblique.

### UpperCase & LowerCase

The **`text-transform`** property
is used to change the case of
text giving it one of the following
values:

* `uppercase`

  This causes the text to appear
uppercase.
* `lowercase`

  This causes the text to appear
lowercase.
* `capitalize`

  This causes the first letter of
each word to appear capitalized.

### Underline & Strike

The **`text-decoration`** property
allows you to specify the
following values:


* `none`

  This removes any decoration
already applied to the text.

* `underline`

  This adds a line underneath the
text.

* `overline`

  This adds a line over the top of
the text.
`line-through
`This adds a line through words.

* `blink`

  This animates the text to make it
flash on and off (however this is
generally frowned upon, as it is
considered rather annoying).


### Leading

Leading (pronounced ledding) is
a term typographers use for the
vertical space between lines of
text. In a typeface, the part of
a letter that drops beneath the
baseline is called a **descender**,
while the highest point of a letter
is called the **ascender**. Leading
is measured from the bottom of
the descender on one line to the
top of the ascender on the next.

### Letter & Word Spacing

**`letter-spacing`**,**` word-spacing`**

### Alignment

The **`text-align`** property allows
you to control the alignment of
text. The property can take one
of four values:

* `left`

  This indicates that the text
should be left-aligned.

* `right`

  This indicates that the text
should be right-aligned.

* `center`

  This allows you to center text.

* `justify`

  This indicates that every line in
a paragraph, except the last line,
should be set to take up the full
width of the containing box.

### CSS3: Drop Shadow

The **`text-shadow`** property has
become commonly used despite
lacking support in all browsers.

### First Lett er or Line

You can specify different values
for the first letter or first line of
text inside an element using

**`:first-letter`** 

and

**`:first-line`**.