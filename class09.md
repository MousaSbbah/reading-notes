[HOME](https://mousasbbah.github.io/reading-notes/) 

# Forms and Events

## Forms 

An HTML form is used to collect user input. The user input is most often sent to a server for processing.

There are several types of form controls that
you can use to collect information from visitors
to your site.

  * **ADDING TEXT:**
    * Text input
    * Password input
    * Text area
  *** Making Choices:**
    * Radio buttons
    * Checkboxes
    * Drop-down boxes
  * **Submitting Forms:**
    * Submit buttons
    * Image buttons

  * **Uploading Files:**
    * File upload

### **The `<form>` Element**
The HTML `<form>` element is used to create an HTML form for user input:
```html
<form>
.
form elements
.
</form>
```

### **The `<input>` Element**
The HTML `<input>` element is the most used form element.

An `<input>` element can be displayed in many ways, depending on the type attribute.

Here are some examples:
|Type	|Description|
|--|--|
`<input type="text">`|	Displays a single-line text input field
`<input type="radio">`	|Displays a radio button (for selecting one of many choices)
`<input type="checkbox">`|	Displays a checkbox (for selecting zero or more of many choices)
`<input type="submit">`|	Displays a submit button (for submitting the form)
`<input type="button">`|	Displays a clickable button


## FORMS CHEAT SHEET
|Forms|
|---|
`<form>` `</form>`<br>Defines a form|
`<select multiple name=? size=?> </select>`<br>Creates a scrolling menu. Size sets the number of menu items visible before user needs to scroll.
`<select name=?> </select>`<br>Creates a pulldown menu
`<option>`<br>Sets off each menu item
`<textarea name=? cols="x" rows="y"></textarea>`<br>Creates a text box area. Columns set the width; rows set the height.
`<input type="checkbox" name=? value=?>`<br>Creates a checkbox.
`<input type="checkbox" name=? value=? checked>`<br>Creates a checkbox which is pre-checked.
`<input type="radio" name=? value=?>`<br>Creates a radio button.
`<input type="radio" name=? value=? checked>`
Creates a radio button which is pre-checked.
`<input type="text" name=? size=?>`<br>Creates a one-line text area. Size sets length, in characters.
`<input type="submit" value=?>`<br>Creates a submit button. Value sets the text in the submit button.
`<input type="image" name=? src=? border=? alt=?>`<br>Creates a submit button using an image.
`<input type="reset">`<br>Creates a reset button

# CSS Lists, Tables and Forms

## LISTS 

### **Bullet Point Styles**

The **`list-style-type`** property
allows you to control the shape
or style of a bullet point (also
known as a marker).

### **Images for Bullets**
You can specify an image to act
as a bullet point using the
**`list-style-image`** property.

### **Positioning the Marker**

Lists are indented into the page
by default and the **`list-styleposition`**
property indicates
whether the marker should
appear on the inside or the
outside of the box containing the
main points.

### **List Shorthand**
As with several of the other CSS
properties, there is a property
that acts as a shorthand for list
styles. It is called **`list-style`**,
and it allows you to express
the markers' style, image and
position properties in any order

## TABLES 


**border-collapse**

`collapse` | `separate`

**empty-cells**

`show` | `hide`

**border-spacing**

`length` `length`

**table-layout**

`auto` | `fixed`

**caption-side**

`top` | `bottom` | `left` | `right`

# JavaScript : Events

HTML events are "things" that happen to HTML elements.

When JavaScript is used in HTML pages, JavaScript can "react" on these events.

An HTML event can be something the browser does, or something a user does.

Here are some examples of HTML events:

* An HTML web page has finished loading
* An HTML input field was changed
* An HTML button was clicked
Often, when events happen, you may want to do something.

JavaScript lets you execute code when events are detected.

## EVENTS CHEAT SHEET

**Mouse**

`onclick`

The event occurs when the user clicks on an element

`oncontextmenu`

User right-clicks on an element to open a context menu

`ondblclick`

The user double-clicks on an element

`onmousedown`

User presses a mouse button over an element

`onmouseenter`

The pointer moves onto an element

`onmouseleave`

Pointer moves out of an element

`onmousemove`

The pointer is moving while it is over an element

`onmouseover`

When the pointer is moved onto an element or one of its children

`onmouseout`

User moves the mouse pointer out of an element or one of its children

`onmouseup`

The user releases a mouse button while over an element

**Keyboard**

`onkeydown`

When the user is pressing a key down

`onkeypress`

The moment the user starts pressing a key

`onkeyup`

The user releases a key

**Frame**

`onabort`

The loading of a media is aborted

`onbeforeunload`

Event occurs before the document is about to be unloaded

`onerror`

An error occurs while loading an external file


`onhashchange`

There have been changes to the anchor part of a URL

`onload`

When an object has loaded

`onpagehide`

The user navigates away from a webpage

`onpageshow`

When the user navigates to a webpage

`onresize`

The document view is resized

`onscroll`

An element’s scrollbar is being scrolled

`onunload`

Event occurs when a page has unloaded

**Form**

`onblur`

When an element loses focus

`onchange`

The content of a form element changes (for `<input>`, `<select>`and `<textarea>`)

`onfocus`

An element gets focus

`onfocusin`

When an element is about to get focus

`onfocusout`

The element is about to lose focus

`oninput`

User input on an element

`oninvalid`

An element is invalid


`onreset`

A form is reset

`onsearch`

The user writes something in a search field (for `<input="search">`)

`onselect`

The user selects some text (for `<input>` and `<textarea>`)

`onsubmit`

A form is submitted

**Drag**

`ondrag`

An element is dragged

`ondragend`

The user has finished dragging the element

`ondragenter`

The dragged element enters a drop target

`ondragleave`

A dragged element leaves the drop target

`ondragover`

The dragged element is on top of the drop target

`ondragstart`

User starts to drag an element

`ondrop`

Dragged element is dropped on the drop target

**Clipboard**

`oncopy`

User copies the content of an element

`oncut`

The user cuts an element’s content


`onpaste`

A user pastes content in an element

**Media**

`onabort`

Media loading is aborted

`oncanplay`

The browser can start playing media (e.g. a file has buffered enough)

`oncanplaythrough`

When browser can play through media without stopping

`ondurationchange`

The duration of the media changes

`onended`

The media has reached its end

`onerror`

Happens when an error occurs while loading an external file

`onloadeddata`

Media data is loaded

`onloadedmetadata`

Meta Metadata (like dimensions and duration) are loaded

`onloadstart`

Browser starts looking for specified media

`onpause`

Media is paused either by the user or automatically

`onplay`

The media has been started or is no longer paused

`onplaying`

Media is playing after having been paused or stopped for buffering

`onprogress`

Browser is in the process of downloading the media

`onratechange`

The playing speed of the media changes

`onseeked`

User is finished moving/skipping to a new position in the media

`onseeking`

The user starts moving/skipping

`onstalled`

The browser is trying to load the media but it is not available

`onsuspend`

Browser is intentionally not loading media

`ontimeupdate`

The playing position has changed (e.g. because of fast forward)

`onvolumechange`

Media volume has changed (including mute)

`onwaiting`

Media paused but expected to resume (for example, buffering)

**Animation**

`animationend`

A CSS animation is complete

`animationiteration`

CSS animation is repeated

`animationstart`

CSS animation has started

**Other**

`transitionend`

Fired when a CSS transition has completed
onmessage

`onoffline`

Browser starts to work offline

`ononline`

The browser starts to work online

`onpopstate`

When the window’s history changes

`onshow`

A `<menu>` element is shown as a context menu

`onstorage`

A Web Storage area is updated

`ontoggle`

The user opens or closes the `<details>` element

`onwheel`

Mouse wheel rolls up or down over an element

`ontouchcancel`

Screen touch is interrupted

`ontouchend`

User finger is removed from a touch screen

`ontouchmove`

A finger is dragged across the screen

`ontouchstart`

Finger is placed on touch screen


[HOME](https://mousasbbah.github.io/reading-notes/) 