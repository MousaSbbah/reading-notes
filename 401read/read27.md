## Review, Research, and Discussion


**Does a deployed React application require a server?**

You don't necessarily need a static server in order to run a Create React App project in production. It also works well when integrated into an existing server side app.

**Why do we prefer to test a React application at the behavior rather than the unit level?**



**What does npm run build do?**

creates a build directory with a production build of your app. Set up your favorite HTTP server so that a visitor to your site is served index.html, and requests to static paths like /static/js/main.`<hash>`.js are served with the contents of the /static/js/main.`<hash>`.js file.

**Describe the actual composition / architecture of a React application**

Composition is the act of combining parts or elements to form a whole.
Components are the UI building blocks in React applications, like pure functions are the building blocks of function composition.


|TERMS||
|---|----|
|BDD|Behaviour Driven Development (BDD) is a synthesis and refinement of practices stemming from Test Driven Development (TDD) and Acceptance Test Driven Development (ATDD). |
|Acceptance testing|a testing technique performed to determine whether or not the software system has met the requirement specifications. The main purpose of this test is to evaluate the system's compliance with the business requirements and verify if it is has met the required criteria for delivery to end users.|
|mounting|is a process by which the operating system makes files and directories on a storage device (such as hard drive, CD-ROM, or network share) available for users to access via the computer's file system.
|
|Build | is the process of creating the application program for a software release, by taking all the relevant source code files and compiling them and then creating a build artefact, such as binaries or executable program, etc.
|

## `setState` explained
React components can, and often do, have state. State can be anything, but think of things like whether a user is logged in or not and displaying the correct username based on which account is active. Or an array of blog posts. Or if a modal is open or not and which tab within it is active.

![](https://i1.wp.com/css-tricks.com/wp-content/uploads/2018/04/image_preview-1.jpeg?w=300&ssl=1)

## Handling Events

- React events are named using camelCase, rather than lowercase.
- With JSX you pass a function as the event handler, rather than a string.
```jsx
<button onClick={activateLasers}>
  Activate Lasers
</button>
```

Another difference is that you cannot return false to prevent default behavior in React. You must call preventDefault explicitly. For example, with plain HTML, to prevent the default form behavior of submitting, you can write:
```jsx
<form onsubmit="console.log('You clicked submit.'); return false">
  <button type="submit">Submit</button>
</form>
```

## forms

This form has the default HTML form behavior of browsing to a new page when the user submits the form. If you want this behavior in React, it just works. But in most cases, it’s convenient to have a JavaScript function that handles the submission of the form and has access to the data that the user entered into the form. The standard way to achieve this is with a technique called “controlled components”.

### Controlled Components

In HTML, form elements such as `<input>`, `<textarea>`, and `<select>` typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().

We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.


### State and Lifecycle

Lifecycle of Components
Each component in React has a lifecycle which you can monitor and manipulate during its three main phases.

- **Mounting**

Mounting means putting elements into the DOM.

React has four built-in methods that gets called, in this order, when mounting a component:
  1. constructor()
  1. getDerivedStateFromProps()
  1. render()
  1. componentDidMount()

- **Updating**

The next phase in the lifecycle is when a component is updated.

A component is updated whenever there is a change in the component's state or props.

React has five built-in methods that gets called, in this order, when a component is updated:

1. getDerivedStateFromProps()
1. shouldComponentUpdate()
1. render()
1. getSnapshotBeforeUpdate()
1. componentDidUpdate()


- **Unmounting**

The next phase in the lifecycle is when a component is removed from the DOM, or unmounting as React likes to call it.

React has only one built-in method that gets called when a component is unmounted:

* componentWillUnmount()


## Components and Props


### React Components

Components are independent and reusable bits of code. They serve the same purpose as JavaScript functions, but work in isolation and return HTML via a render() function.

Components come in two types, Class components and Function components

### React Props

React Props are like function arguments in JavaScript and attributes in HTML.


## 

