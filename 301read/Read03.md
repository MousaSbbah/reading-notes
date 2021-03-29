# MUSTACHE 
![MUSTACHE](https://miro.medium.com/max/875/1*P9q0tkeaRY2l1JOXaVKAig.png)
Mustache is a logic-less template syntax. It can be used for HTML, config files, source code — anything. It works by expanding tags in a template using values provided in a hash or object.

```
Mustache.render(“Hello, {{name}}”, { name: “Sherlynn” });

// returns: Hello, Sherlynn
```

In the above, we see two braces around {{ name }}. This is Mustache syntax to show that it is a placeholder. When Mustache compiles this, it will look for the ‘name’ property in the object we pass in, and replace {{ name }} with the actual value, e,g, “Sherlynn”.

#  Flexbox

CSS Flexbox Layout Module
Before the Flexbox Layout module, there were four layout modes:

Block, for sections in a webpage
Inline, for text
Table, for two-dimensional table data
Positioned, for explicit position of an element
The Flexible Box Layout Module, makes it easier to design flexible responsive layout structure without using float or positioning.

## Flex Parent
The flex container becomes flexible by setting the display property to flex:

```css
.flex-container {
  display: flex;
}
```

The flex container properties are:

* **flex-direction**

  The flex-direction property defines in which direction the container wants to stack the flex items.
* **flex-wrap**
  
  The flex-wrap property specifies whether the flex items should wrap or not.
* **flex-flow**
  
  The flex-flow property is a shorthand property for setting both the flex-direction and flex-wrap properties.
* **justify-content**

  The justify-content property is used to align the flex items
* **align-items**

  The align-items property is used to align the flex items.
* **align-content**

  The align-content property is used to align the flex lines.


## Flex Items

The flex item properties are:

* **order**

  The order property specifies the order of the flex items.
* **flex-grow**

  The flex-grow property specifies how much a flex item will grow relative to the rest of the flex items.


* **flex-shrink**

  The flex-shrink property specifies how much a flex item will shrink relative to the rest of the flex items.
* **flex-basis**

  The flex-basis property specifies the initial length of a flex item.
* **flex**

  The flex property is a shorthand property for the flex-grow, flex-shrink, and flex-basis properties.
* **align-self**

  The align-self property specifies the alignment for the selected item inside the flexible container.