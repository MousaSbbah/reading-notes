# Regular Expressions

A regular expression is a sequence of characters that forms a search pattern.

The search pattern can be used for text search and text replace operations.

## What Is a Regular Expression?
A regular expression is a sequence of characters that forms a search pattern.

When you search for data in a text, you can use this search pattern to describe what you are searching for.

A regular expression can be a single character, or a more complicated pattern.

Regular expressions can be used to perform all types of text search and text replace operations.




# Grid Layout Module

## Grid Layout
The CSS Grid Layout Module offers a grid-based layout system, with rows and columns, making it easier to design web pages without having to use floats and positioning.

## Display Property
An HTML element becomes a grid container when its `display `property is set to `grid` or `inline-grid`.

Example
```css
.grid-container {
  display: grid;
}
```

You can adjust the gap size by using one of the following properties:

* grid-column-gap
* grid-row-gap
* grid-gap


Example
```css
.grid-container {
  display: grid;
  grid-column-gap: 50px;
}
```




## Child Elements (Items)
A grid container contains grid items.

By default, a container has one grid item for each column, in each row, but you can style the grid items so that they will span multiple columns and/or rows.



