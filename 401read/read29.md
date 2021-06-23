#  Routing

## Review, Research, and Discussion


**Do child components have direct access to props/state from the parent?**

yes

**When a component “wraps” another component, how does the child component’s output get rendered?**

```jsx
<Main>
  <Content />
</Main>
```
Can a component, such as ``<Content />``, which is a child also be used as a standalone component elsewhere in the application?

yes

What trick can a parent use to share all props with it’s children

Cloning children with new props


## Document the following Vocabulary Terms

|Term||
|---|---|
|props.children|props. children does is that it is used to display whatever you include between the opening and closing tags when invoking a component. A simple example: Here's an example of a stateless function that is used to create a component|
|composition|React Composition is a development pattern based on React's original component model where we build components from other components using explicit defined props or the implicit children prop|


# ReactJS Routing
Routing is the process where user is directed to or rendered different pages based on user action/requests. In React, we can build Single Page Application (SPA) where web app loads a single page and dynamically updates that page as the user interacts with the web app.
## ReactJS Router
ReactJS supports Single Page Application (SPA) using react router package. Router package helps directing users to different pages based on the url. When a user requests a specific url, the routing engine captures that url and renders the view based on the routes defined without reloading the entire application.
## React Router Installation
React Router comes into three different packages react-router, react-router-dom, and react-router-native with it. The react-router package enables the core routing components and functions for React Router applications, we never need to install it directly. The other two react-router-dom (browser specific) and react-router-native are environment specific. Since, we are building a web application, so we will install react-router-dom.

## React Router Installation
React Router comes into three different packages `react-router`, `react-router-dom`, and `react-router-native` with it. The `react-router` package enables the core routing components and functions for React Router applications, we never need to install it directly. The other two `react-router-dom `(browser specific) and `react-router-native `are environment specific. Since, we are building a web application, so we will install react-router-dom.

# Example: 

```jsx

import React, { Component } from 'react';
import { BrowserRouter as Router, Route, Link } from "react-router-dom";
 
const Home = () => {
  return (
    <div>
      <p>Home</p>
    </div>
  );
};
 
const About = () => {
  return (
    <div>
      <p>About</p>
    </div>
  );
};
 
const Contact = () => {
  return (
    <div>
      <p>Contact</p>
    </div>
  );
};
class App extends Component {
  render() {
    return (
        <Router>
              <div>
              <h1>W3Adda - Simple SPA</h1>
                <nav>
                  <ul>
                    <li>
                      <Link to="/">Home</Link>
                    </li>
                    <li>
                      <Link to="/about">About</Link>
                    </li>
                    <li>
                      <Link to="/contact">Users</Link>
                    </li>
                  </ul>
                </nav>
 
                <Route path="/" exact component={Home} />
                <Route path="/about" component={About} />
                <Route path="/contact" component={Contact} />
              </div>
        </Router>
    );
  }
}
 
export default App;
```

## [browser router api docs (read-->)](https://reacttraining.com/react-router/web/api)