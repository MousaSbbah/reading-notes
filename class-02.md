[Home Page](https://mousasbbah.github.io/reading-notes)


# **HTML**


##  **TEXT**
***

### **Headings and paragraphs**

1. Heading

   HTML has **six "levels"** of
headings:
   ```  
     <h1>
     <h2>
     <h3>
     <h4>
     <h5>
     <h6>
   ```
   `<h1>` is used for main headings
`<h2>` is used for subheadings
If there are further sections
under the subheadings then the
`<h3>` element is used, and so
on...

   Browsers display the contents of
headings at different sizes. The
contents of an `<h1>` element is
the largest, and the contents of
an `<h6`> element is the smallest.
The exact size at which each
browser shows the headings
can vary slightly. Users can also
adjust the size of text in their
browser. You will see how to
control the size of text, its color,
and the fonts used when we
come to look at CSS.

2. paragraph
 
    **`<p>`**

   To create a paragraph, surround
the words that make up the
paragraph with an opening `<p>`
tag and closing `</p>` tag.
By default, a browser will show
each paragraph on a new line
with some space between it and
any subsequent paragraphs.


### **Bold & Italic**

1. bold 

   `<b>`
By enclosing words in the tags
`<b>` and `</b>` we can make
characters appear bold.



2. Italic

   By enclosing words in the tags
`<i>` and `</i>` we can make
characters appear italic.


### **Superscript &Subscript**
   

The `<sup>` element is used
to contain characters that
should be superscript such
as the suffixes of dates or
mathematical concepts like
raising a number to a power such
as

` 2<sup>2</sup>`  -------> 2<sup>2</sup>



The `<sub>` element is used to
contain characters that should
be subscript. It is commonly
used with foot notes or chemical
formulas such as 

`H<sub>2</sub>0`   ----->  H<sub>2</sub>0.

### **Line Breaks & Horizontal Rules**

* As you have already seen, the
browser will automatically show
each new paragraph or heading
on a **new line**. But if you wanted
to add a line break inside the
middle of a paragraph you can
use the line break tag  `<br />`.

* To create a break between
themes — such as a change of
topic in a book or a new scene
in a play — you can add a
horizontal rule between sections
using the `<hr />` tag.

## **Semantic Markup**
There are some text elements that are not intended to affect the
structure of your web pages, but they do add extra information to the
pages — they are known as semantic markup.

### **Strong & Emphasis**

 * The use of the `<strong>`
element indicates that its
content has strong importance.
For example, the words
contained in this element might
be said with strong emphasis.<br>
By default, browsers will show
the contents of a `<strong>`
element in bold.
* The `<em>` element indicates
emphasis that subtly changes
the meaning of a sentence.
By default browsers will show
the contents of an `<em>` element
in italic.

### **Quotations**

* `<blockquote>`

  The `<blockquote>` element is
used for longer quotes that take
up an entire paragraph. Note
how the `<p>` element is still
used inside the `<blockquote>`
element.

* `<q>`

   The `<q>` element is used for
shorter quotes that sit within
a paragraph. Browsers are
supposed to put quotes around
the `<q>` element, however
Internet Explorer does not —
therefore many people avoid
using the `<q>` element.

### **Abbreviations & Acronyms**
 * `<abbr>`

     
   If you use an abbreviation or
an acronym, then the `<abbr>`
element can be used. A title
attribute on the opening tag is
used to specify the full term.
### **Citations & Definitions**
* **`<cite>`**

   When you are referencing a
piece of work such as a book,
film or research paper, the
`<cite>` element can be used
to indicate where the citation is
from.
* **`<dfn>`**

   The first time you explain some
new terminology (perhaps an
academic concept or some
jargon) in a document, it is
known as the defining instance
of it.
The `<dfn>` element is used to
indicate the defining instance of
a new term.

### **Author Details**

* `<address>` 

   The `<address>` element has
quite a specific use: to contain
contact details for the author of
the page.
It can contain a physical address,
but it does not have to. For
example, it may also contain a
phone number or email address.

----
# CSS

## **What CSS does?**
CSS allows you to create rules that specify how the content of
an element should appear. For example, you can specify that
the background of the page is cream, all paragraphs should
appear in gray using the Arial typeface, or that all level one
headings should be in a blue, italic, Times typeface.

## Using External CSS `<link>` 


The `<link>` element can be used
in an HTML document to tell the
browser where to find the CSS
file used to style the page. It is an
empty element (meaning it does
not need a closing tag), and it
lives inside the `<head>` element.
It should use three attributes:


**href**

This specifies the path to the
CSS file (which is often placed in
a folder called css or styles).

**type**

This attribute specifies the type
of document being linked to. The
value should be text/css.

**rel**

This specifies the relationship
between the HTML page and
the file it is linked to. The value
should be stylesheet when
linking to a CSS file.

## Using Internal CSS `<style>`


You can also include CSS rules
within an HTML page by placing
them inside a `<style>` element,
which usually sits inside the
`<head`> element of the page.
The `<style>` element should use
the type attribute to indicate
that the styles are specified in
CSS. The value should be text/
css.


****
 When building a site with more
than one page, you should use
an external CSS style sheet. This:
   * Allows all pages to use the
same style rules (rather than
repeating them in each page).
   * Keeps the content separate
from how the page looks.
  * Means you can change the
styles used across all pages
by altering just one file
(rather than each individual
page).

## CSS Selectors
There are many different types
of **CSS selector** that allow you to
target rules to specific elements
in an HTML document.
The table below introduces the most commonly
used CSS selectors.

|Selector|Meaning|Example|
|---|---|---|
|Universal Selector|Applies to all elements in the document|`* {}`<br> Targets all elements on the page|
|Type Selector|Matches element names|`h1, h2, h3 {}`<br>Targets the `<h1>`, `<h2>` and `<h3>` elements|
|Class Selector|Matches an element whose class attribute has a value that matches the one specified after the period (or full stop) symbol|`.note {}`<br> Targets any element whose class attribute has a value of note<br> `p.note {}`<br> Targets only `<p>` elements whose class attribute has a value of note|
|ID Selector|Matches an element whose id attribute has a value that matches the one specified afterthe pound or hash symbol|`#introduction {}`<br> Targets the element whose id attribute has a value of introduction|
***
## Why use External Style Sheets?

   * All of your web pages can share
the same style sheet.
* If you want to make a
change to how your site appears,
you only need to edit the one
CSS file and all of your pages
will be updated
* If you are just creating a single
page, you might decide to put
the rules in the same file to
keep everything in one place.


---





# JAVA script basics

 ## STATEMENTS

 A script is a series of instructions that a computer can follow one-by-one.
Each individual instruction or step is known as a statement.
Statements should end with a semicolon.

##  COMMENTS 

You should write comments to explain what your code does.
They help make your code easier to read and understand.
This can help you and others who read your code.
 for example :
 ``` 
 /* (MULTI-LINE COMMENTS example )This script displays a greeting to the user based upon the current time.*/
  
```
` //SINGLE-LINE COMMENTS`

 ## VARIABLES

 A script will have to temporarily
store the bits of information it
needs to do its job. It can store this
data in variables.

JavaScript distinguishes between numbers,
strings, and true or false values known as
Booleans.
   * **NUMERIC DATA TYPE**

     The numeric data type handles
numbers.
* **STRING DATA TYPE**

  The strings data type consists of
letters and other characters.
* **BOOLEAN DATA TYPE**

   Boolean data types can have one
of two va lues: true or false.

## ARRAYS 
An array is a special type of variable. It doesn't
just store one value; it stores a list of values.You should consider using an
array whenever you are working
with a **list** or a set of values that
are **related** to each other.Arrays are especially helpful
when you do not know how
many items a list will contain
because, when you create the
array, you do not need to specify
how many values it will hold.

### CREATING AN ARRAY
*  You create an array and give it
a name just like you would any
other variable (using the var
keyword followed by the name of
the array).
The values are assigned to the
array inside a pair of square
brackets, and each value is
separated by a comma. The
values in the array do not need
to be the same data type, so you
can store a string, a number and
a Boolean all in the same array.

   for example :

   `var
colors ['white', 'black', ' custom '];`


### VALUES IN ARRAYS

Values in an array are accessed as if they are in
a numbered list. It is important to know that the
numbering of this list starts at zero (not one).

### ACCESSING & CHANGING VALUES IN AN ARRAY

To access a value from an array,
after the array name you specify
the index number for that value
inside square brackets.
You can change the value of an
item an array by selecting it and
assigning it a new value just as
you would any other variable
(using the equals sign and the
new value for that item).

## EXPRESSIONS

An expression evaluates into (results in) a single value. Broadly speaking
there are two types of expressions.

   * **EXPRESSIONS THAT JUST ASSIGN A VALUE TO A VARIABLE**

      for example :` var color = 'beige';`
    
* **EXPRESSIONS THAT USE TWO OR MORE VALUES TO RETURN A SINGLE VALUE**

    for example : `var area = 3 * 2;`

## Operators
Expressions rely on things called operators; they allow programmers to
create a single value from one or more values.
### ARITHMETIC OPERATORS
JavaScript contains the following mathematical
operators, which you can use with numbers.

|Operator| Name|
|--|--|
|ADDITION| +|
|SUBTRACTION|- |
|DIVISION|/|
|MULTIPLICATION|* |
|INCREMENT| ++|
|DECREMENT| --|
|MODULUS| %|



# JAVA script Decisions & Loops

### Comparison Operators : Evaluating Conditions

1. **`==`**  is equal to 

2. **`!=`** is not equal to 
3. **`===`**  strict equal to 
4. **`!==`** strict not equal to 
5. **`>`** Greater than 
6. **`<`** Less than
7. **`>=`** Greater than or equal to
8. **`<=`** Less than or equal to

### Logical Operators

1. **`&&`** Logical **AND**
2. **`||`** Logical **OR**
3. **`!`** Logical **NOT**


## IF STATEMENT 

The if statement evaluates (or checks) a condition. If the condition 
evaluates to true, any statements in the subsequent code block are 
executed. 

``` 
if (condition) {
  //  block of code to be executed if the condition is true
}

```

* If the condition evaluates to **true**, the following 
code block (the code in the next set of curly braces) 
is executed. 
* If the condition resolves to **false** the statements in 
that code block are not run. (The script continues to 
run from the end of the next code block.)

## IF ... ELSE STATEMENT

The if.. else statement checks a condition. 
If it resolves to true the first code block is executed. 
If the condition resolves to false the second code block is run instead. 

``` 
if (condition) {
  //  block of code to be executed if the condition is true
} else {
  //  block of code to be executed if the condition is false
}



```





















