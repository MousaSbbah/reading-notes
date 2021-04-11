# EJS

 EJS is a simple templating language that lets you generate HTML markup with plain JavaScript.

![aaa](https://miro.medium.com/max/3920/1*VMI-NGFtYwWM7aBoKOg72Q.jpeg)
 ## Features 


* Fast compilation and rendering
* Simple template tags: <% %>
* Custom delimiters (e.g., use [? ?] instead of <% %>)
* Sub-template includes
* Ships with CLI
* Both server JS and browser support
* Static caching of intermediate JavaScript
* Static caching of templates
* Complies with the Express view system


![asaf](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRaj9fzRDELsW_iLoKQGV9wfGLthg3Ty_M-Gg&usqp=CAU)
 ## Install
It's easy to install EJS with NPM.

```
$ npm install ejs
```

## Examples

```html
<script src="ejs.js"></script>
<script>
  let people = ['geddy', 'neil', 'alex'];
  let html = ejs.render('<%= people.join(", "); %>', {people: people});
</script>
```


```html
<% if (user) { %>
  <h2><%= user.name %></h2>
<% } %>

```


## Tags
* `<%` 'Scriptlet' tag, for control-flow, no output
* `<%_` ‘Whitespace Slurping’ Scriptlet tag, strips all whitespace before it
* `<%=` Outputs the value into the template (HTML escaped)
* `<%-` Outputs the unescaped value into the template
* `<%#` Comment tag, no execution, no output
* `<%%` Outputs a literal '<%'
* `%>` Plain ending tag
* `-%>` Trim-mode ('newline slurp') tag, trims following newline
* `_%>` ‘Whitespace Slurping’ ending tag, removes all whitespace after it



