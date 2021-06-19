# Component Based UI

### **Review, Research, and Discussion**

- **Name 5 Javascript UI Frameworks (other than React)**
    - Angular
    - Vue
    - Ember
    - Svelte 3
    - Ext JS by Sencha
- **What’s the difference between a framework and a library?**
    The key difference between JavaScript libraries and frameworks is that libraries consist of functions that an application can call to perform a task, while a framework defines how a developer designs an application. In other words, the framework calls on the application code, rather than the other way around.

#### **Term**
|Terms||
|--|--|
|Rendering|It is a process of generating HTML output which is ready to be rendered by web browser and viewable by user, this process can happen anywhere and anytime depending on your strategy.|
|Templates|![](https://miro.medium.com/max/625/1*0VAaNhnCrDFkSpq8MyjmqQ.png)|
|State|The state is an instance of React Component Class can be defined as an object of a set of observable properties that control the behavior of the component.|

## **REACT** 

### Hello World

The smallest React example looks like this:

```js
ReactDOM.render(
  <h1>Hello, world!</h1>,
  document.getElementById('root')
);
```

### Introducing JSX

It is called JSX, and it is a syntax extension to JavaScript. We recommend using it with React to describe what the UI should look like. JSX may remind you of a template language, but it comes with the full power of JavaScript.

Example : 

```jsx
const name = 'Josh Perez';
const element = <h1>Hello, {name}</h1>;

ReactDOM.render(
  element,
  document.getElementById('root')
);

```

### Rendering Elements


**Rendering an Element into the DOM**

Let’s say there is a <div> somewhere in your HTML file:

``` html
<div id="root"></div> 
```

To render a React element into a root DOM node, pass both to `ReactDOM.render()`:

```js
const element = <h1>Hello, world</h1>;
ReactDOM.render(element, document.getElementById('root'));
```

**Updating the Rendered Element**

React elements are immutable. Once you create an element, you can’t change its children or attributes. An element is like a single frame in a movie: it represents the UI at a certain point in time.

With our knowledge so far, the only way to update the UI is to create a new element, and pass it to ``ReactDOM.render()``.

Example : 

```js
function tick() {
  const element = (
    <div>
      <h1>Hello, world!</h1>
      <h2>It is {new Date().toLocaleTimeString()}.</h2>
    </div>
  );
  ReactDOM.render(element, document.getElementById('root'));
}

setInterval(tick, 1000);
```

   ``**React Only Updates What’s Necessary**``