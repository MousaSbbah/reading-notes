[Home Page](https://mousasbbah.github.io/reading-notes)


# Color 

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

## CSS3 OPACITY
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

## CSS3 HSL & HSLA

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