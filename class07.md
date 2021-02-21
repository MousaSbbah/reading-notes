 [HOME](https://mousasbbah.github.io/reading-notes/) 

# HTML Tables; JS Constructor Functions


## TABLES 

**What's a Table?**

A table represents information in a grid format.
Examples of tables include financial reports, TV
schedules, and sports results.

### **Basic Table Structure**

**`<table>`**

The `<table>` element is used
to create a table. The contents
of the table are written out row
by row.

**`<tr>`**

You indicate the start of each
row using the opening `<tr>` tag.
(The tr stands for table row.)
It is followed by one or more
`<td>` elements (one for each cell
in that row).

At the end of the row you use a
closing `</tr>` tag.

**`<td>`**

Each cell of a table is
represented using a `<td>`
element. (The td stands for
table data.)

At the end of each cell you use a
closing `</td> `tag.

**Table Headings**

**`<th>`**

The `<th>` element is used just
like the `<td>` element but its
purpose is to represent the
heading for either a column or
a row. (The th stands for table
heading.)

**Spanning ColumnS**

Sometimes you may need the
entries in a table to stretch
across more than one column.

The **`colspan`** attribute can be
used on a `<th>` or `<td>` element
and indicates how many columns
that cell should run across.

**Spanning Rows**

You may also need entries in
a table to stretch down across
more than one row.

The **`rowspan`** attribute can be
used on a `<th>` or `<td>` element
to indicate how many rows a cell
should span down the table.

## Long Tables

**`<thead>`**

The headings of the table should
sit inside the `<thead>` element.

**`<tbody>`**

The body should sit inside the
`<tbody>` element.

**`<tfoot>`**

The footer belongs inside the
`<tfoot>` element.
***
## Functions, Methods, and Objects

### **CREATE THE OBJECT, THEN ADD PROPERTIES & METHODS**

#### LITERAL NOTATION
```js
var hotel = {}
hotel .name= 'Quay';
hotel .rooms = 40;
hotel.booked = 25;
hotel.checkAvailabil ity =function()
return this . rooms - this .booked;
} ;
```

#### OBJECT CONSTRUCTOR NOTATION
```js
var hotel = new Object();
hotel.name = 'Quay';
hotel .rooms = 40 ;
hotel . booked= 25;
hotel.checkAvailability =function()
return this .rooms - this .booked;
} ;

```
### **CREATING AN OBJECT WITH PROPERTIES & METHODS**
#### LITERAL NOTATION
```js
var hotel = {
name: 'Quay' ,
rooms: 40,
booked: 25,
chec kAvailability: function() {
return this.rooms - this .booked;
}
} ;
```
#### OBJECT CONSTRUCTOR NOTATION
```js
function Hotel(name, rooms, booked) {
this.name = name;
th i s.rooms = rooms;
this.booked = booked;
this.checkAvailability = functio n()
return this . rooms - this.booked;
} ;
var quayHotel =new Hotel('Quay', 40 , 25);
var parkHotel =new Hotel('Park', 120, 77);
```

### **THE DOCUMENT OBJECT MODEL: THE DOCUMENT OBJECT**

The topmost object in the Document Object Model (or DOM) is the
document object. It represents the web page loaded into the current
browser window or tab.

Here are some properties of the
document object, which tell you
about the current page.

|PROPERTY|DESCRIPTION|
|---|---|
|`document.title`|Title of current document|
|`document.lastModified`|Date on which document was last modified|
|`document .URL`|Returns string containing URL of current document|
|`document.domain`|Returns domain of current document|

The following are a few of the
methods that select content or
update the content of a page.

|METHOD|DESCRIPTION|
|---|---|
|`document.write()`|Writes text to document|
|`document.getElementById()`|Returns element, if there is an element with the value of the id attribute that matches|
|`document.querySelectorA11()`|Returns list of elements that match a CSS selector, which is specified asa parameter |
|`document.createElement()`|Creates new element|
|`document.createTextNode()`|Creates new text node|

 [HOME](https://mousasbbah.github.io/reading-notes/) 