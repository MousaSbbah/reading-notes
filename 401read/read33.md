# Context API



## Review, Research, and Discussion


**Describe use cases for useMemo() and useReducer()**

The useMemo is a hook used in the functional component of react that returns a memoized value. 

useReducer is a React hook function that accepts a reducer function, and an initial state. ... This hook function returns an array with 2 values. The first one is the state value, and the second value is the dispatch function which is further used to trigger an action with the help of array destructuring

**Why do custom hooks need the use prefix?**

------

**What do custom hooks usually do?**

Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks.

**Using any list of custom hooks, research and name one that you think will be useful in your applications**

useArray hook


**Describe how a hook that fetches API data might work**

---



|Term||
|---|--|
|reducer| a function that determines changes to an application's state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application's state changes in a single store so that they behave consistently|


# Context
![](https://bs-uploads.toptal.io/blackfish-uploads/blog/post/seo/og_image_file/og_image/16097/react-context-api-4929b3703a1a7082d99b53eb1bbfc31f.png)
**Context provides a way to pass data through the component tree without having to pass props down manually at every level.**

In a typical React application, data is passed top-down (parent to child) via props, but such usage can be cumbersome for certain types of props (e.g. locale preference, UI theme) that are required by many components within an application. Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree.

![](https://miro.medium.com/max/3472/1*Jx8BCxZFN2SCuhQtZqfgMQ.jpeg)
## When to Use Context
Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.