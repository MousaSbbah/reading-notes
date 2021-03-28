# jQuery

## What is jQuery
jQuery is a lightweight, "write less, do more", JavaScript library.

The purpose of jQuery is to make it much easier to use JavaScript on your website.

jQuery takes a lot of common tasks that require many lines of JavaScript code to accomplish, and wraps them into methods that you can call with a single line of code.

jQuery also simplifies a lot of the complicated things from JavaScript, like AJAX calls and DOM manipulation.

The jQuery library contains the following features:

* HTML/DOM manipulation
* CSS manipulation
* HTML event methods
* Effects and animations
* AJAX
* Utilities

## jQuery Syntax
The jQuery syntax is tailor-made for selecting HTML elements and performing some action on the element(s).

Basic syntax is: $(selector).action()

* A `$` sign to define/access jQuery
* A (selector) to "query (or find)" HTML elements
* A jQuery action() to be performed on the element(s)

## Set Content - text(), html(), and val()
We will use the same three methods from the previous page to set content:

`text()` - Sets or returns the text content of selected elements
`html()` - Sets or returns the content of selected elements (including HTML markup)
`val() `- Sets or returns the value of form fields
The following example demonstrates how to set content with the jQuery text(), html(), and val() methods:

Example
```js
$("#btn1").click(function(){
  $("#test1").text("Hello world!");
});
$("#btn2").click(function(){
  $("#test2").html("<b>Hello world!</b>");
});
$("#btn3").click(function(){
  $("#test3").val("Dolly Duck");
});
```

## Add New HTML Content
We will look at four jQuery methods that are used to add new content:

`append()` - Inserts content at the end of the selected elements
`prepend()` - Inserts content at the beginning of the selected elements
`after()` - Inserts content after the selected elements
`before() `- Inserts content before the selected elements
jQuery append() Method
The jQuery append() method inserts content AT THE END of the selected HTML elements.

![append](/image/append.bmp)


## Set Attributes - attr()
The jQuery attr() method is also used to set/change attribute values.

The following example demonstrates how to change (set) the value of the href attribute in a link:

Example
```js
$("button").click(function(){
  $('google').attr("href", "https://www.google.com");
});
```
## jQuery Event Methods

All the different visitors' actions that a web page can respond to are called events.

An event represents the precise moment when something happens.

Examples:

* moving a mouse over an element
* selecting a radio button
* clicking on an element

Here are some common DOM events:

|Mouse Events|	Keyboard Events|	Form Events	|Document/Window Events|
|--|-|-|-|
|click	|keypress	|submit	|load|
|dblclick	|keydown|	change|	resize|
|mouseenter|	keyup	|focus|	scroll|
|mouseleave	| |	blur|	unload|


## The `on()` Method
The `on()` method attaches one or more event handlers for the selected elements.

# PAIR PROGRAMMING
***Pair programming*** is an agile software development technique in which two programmers work together at one workstation. One, the **driver**, writes code while the other, the observer or **navigator**, reviews each line of code as it is typed in. The two programmers switch roles frequently.

While reviewing, the observer also considers the "strategic" direction of the work, coming up with ideas for improvements and likely future problems to address. This is intended to free the driver to focus all of their attention on the "tactical" aspects of completing the current task, using the observer as a safety net and guide.