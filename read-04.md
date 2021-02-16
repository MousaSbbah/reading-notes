[Home Page](https://mousasbbah.github.io/reading-notes)


# HTML & CSS
## Links 
Links are the defining feature of the web
because they allow you to move from
one web page to another — enabling the
very idea of browsing or surfing.

### **Writing Links**
Links are created using the `<a>` element. Users can click on anything
between the opening `<a> `tag and the closing `</a>` tag. You specify
which page you want to link to using the href attribute.
Writing Links, For  Example :

```html
<a href="http://www.imdb.com">IMDB</a>
```


  *  **Linking to Other Sites**

     Links are created using the `<a>`
element which has an attribute
called href. The value of the
href attribute is the page that
you want people to go to when
they click on the link.
Users can click on anything that
appears between the opening
`<a>` tag and the closing `</a>`
tag and will be taken to the page
specified in the href attribute.
  * **Linking to Other Pages on the Sa me Site**

     When you are linking to other
pages within the same site,
you do not need to specify the
domain name in the URL. You
can use a shorthand known as a
relative URL.
If all the pages of the site are in
the same folder, then the value
of the href attribute is just the
name of the file.

* **Email Links**
   
     To create a link that starts up
the user's email program and
addresses an email to a specified
email address, you use the `<a>`
element. However, this time the
value of the href attribute starts
with **`mailto`**: and is followed by
the email address you want the
email to be sent to.

* **Opening Links in a New Window**

  If you want a link to open in a
new window, you can use the
**`target`** attribute on the opening
`<a>` tag. The value of this
attribute should be _blank.

## Layout in CSS

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

# JavaScript

## Functions

Functions let you group a series of statements together to perform a
specific task. If different parts of a script repeat the same task, you can
reuse the function (rather than repeating the same set of statements). 

<br>

### Function declarations
A function definition (also called a function declaration, or function statement) consists of the `function` keyword, followed by:

   * The name of the function.
   * A list of parameters to the function, enclosed in parentheses and separated by commas.
   * The JavaScript statements that define the function, enclosed in curly brackets, {...}.

For example :

`` function square(number) {
  return number * number;
}``

### Calling functions
Defining a function does not execute it. Defining it names the function and specifies what to do when the function is called.

Calling the function actually performs the specified actions with the indicated parameters. For example, if you define the function square, you could call it as follows:

`` square(5); ``

## 6 Reasons for Pair Programming

1. **Greater efficiency**

   It is a common misconception that pair programming takes a lot longer and is less efficient. In reality, when two people focus on the same code base, it is easier to catch mistakes in the making. Research indicates that pair programing takes slightly longer, but produces higher-quality code that doesn’t require later effort in troubleshooting and debugging (let alone exposing users to a broken product). So, in the long-run, it’s often actually more efficient than two people working on separate features. When coming up with ideas and discussing solutions out loud, two programmers may come to a solution faster than one programmer on their own. Also, when the pair is stuck, both programmers can research the problem and reach a solution faster. Researches also identified pairing enhances technical skills, team communication, and even enjoy ability of coding in the workplace.

2. **Engaged collaboration**

   When two programmers focus on the same code, the experience is more engaging and both programmers are more focused than if they were working alone. It is harder to procrastinate or get off track when someone else is relying on you to complete the work. Popping open your Facebook timeline is just that less enticing when someone else is looking at your screen.


3. **Learning from fellow students**


   Everyone has a different approach to problem solving; working with a teammate can expose developers to techniques they otherwise would not have thought of. If one developer has a unique approach to a specific problem, pair programming exposes the other developer to a new solution.



4. **Social skills**

   Pair programming is great for improving social skills. When working with someone who has a different coding style, communication is key. This can become more difficult when two programmers have different personalities. Pair programming not only improves programming skills, but can also help programmers develop their interpersonal skills. When just grabbing the keyboard and taking over isn’t an option, getting good at finding the right words is a skill unto itself.


5. **Job interview readiness**

   A common step in many interview processes involves pair programming between a current employee and an applicant, either in person or through a shared screen. They will carry out exercises together, such as code challenges, building a project or feature, or debugging an existing code base. By doing so, companies can get a better feel for how an applicant will fit into the team and their collaboration style.



6. **Work environment readiness**


   Many companies that utilize pair programing expect to train fresh hires from CS-degree programs on how they operate to actually deliver a product. Code Fellows graduates who are already familiar with how pairing works can hit the ground running at a new job, with one less hurdle to overcome. 


    
