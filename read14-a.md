[HOME](https://mousasbbah.github.io/reading-notes/)


# Transforms

With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the transform property.

The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.


## 2D Transforms

* **2D Rotate**

  he transform property accepts a handful of different values. The rotate value provides the ability to rotate an element from 0 to 360 degrees. Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise. The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically.

* **2D Scale**

  Using the scale value within the transform property allows you to change the appeared size of an element. The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger.


* **2D Translate**

  The translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document. Using the translateX value will change the position of an element on the horizontal axis while using the translateY value will change the position of an element on the vertical axis.

* **2D Skew**

  The last transform value in the group, skew, is used to distort elements on the horizontal axis, vertical axis, or both. The syntax is very similar to that of the scale and translate values. Using the skewX value distorts an element on the horizontal axis while the skewY value distorts an element on the vertical axis. To distort an element on both axes the skew value is used, declaring the x axis value first, followed by a comma, and then the y axis value.

 # Transitions & Animations

One evolution with CSS3 was the ability to write behaviors for transitions and animations. Front end developers have been asking for the ability to design these interactions within HTML and CSS, without the use of JavaScript or Flash, for years. Now their wish has come true.

## **Transitions**

As mentioned, for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the `:hover`, `:focus`,` :active`, and `:target` pseudo-classes.

There are four transition related properties in total, including `transition-property`, `transition-duration`, `transition-timing-function`, and `transition-delay`. Not all of these are required to build a transition, with the first three are the most popular.

## Transitional Properties
It is important to note, not all properties may be transitioned, only properties that have an identifiable halfway point. Colors, font sizes, and the alike may be transitioned from one value to another as they have recognizable values in-between one another. The display property, for example, may not be transitioned as it does not have any midpoint. A handful of the more popular transitional properties include the following.
```css
background-color
background-position
border-color
border-width
border-spacingbottom
clip
color
crop
font-size
font-weight
height
left
letter-spacing
line-height
margin
max-height
max-width
min-height
min-width
opacity
outline-color
outline-offsetout
line-width
padding
righttext-indent
text-shadow
topvertical-align
visibility
width
word-spacing
z-index
```

# Examples 
```html
<!DOCTYPE html>
<html>
<head>
    <style type="text/css">
    </style>
</head>
<body>
    <div></div>
</body>
</html>
```

```html
<style type="text/css">
body > div
{
            width:483px;
            height:298px;
            background:#676470;
            transition:all 0.3s ease;
}
</style>
```
## **Fade in**
Having things fade in is a fairly common request from clients. It’s a great way to emphasize functionality or draw attention to a call to action.
```css
.fade
{
        opacity:0.5;
}
.fade:hover
{
        opacity:1;
}
```
## **Change color**
Animating a change of color used to be unbelievably complex, with all kinds of math involved in calculating separate RGB values and then recombining them. 
```css
.color:hover
{
        background:#53a7ea;
}
```
## **Grow & Shrink**
To grow an element, you used to have to use its width and height, or its padding. But now we can use CSS3’s transform to enlarge.
```css
.grow:hover
{
        -webkit-transform: scale(1.3);
        -ms-transform: scale(1.3);
        transform: scale(1.3);
}
```
## **Rotate elements**
CSS transforms have a number of different uses, and one of the best is transforming the rotation of an element. Give your div the class “rotate” and add the following to your CSS:
```css
.rotate:hover
{
        -webkit-transform: rotateZ(-30deg);
        -ms-transform: rotateZ(-30deg);
        transform: rotateZ(-30deg);
}
```
## **Square to circle**
A really popular effect at the moment is transitioning a square element into a round one, and vice versa. With CSS, it’s a simple effect to achieve, we just transition the border-radius property.
```css
.circle:hover
{
        border-radius:50%;
}

```


[HOME](https://mousasbbah.github.io/reading-notes/)