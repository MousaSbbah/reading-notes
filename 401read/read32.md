# Custom Hooks




## Review, Research, and Discussion

**What does a component’s lifecycle refer to?**

Every React Component has a lifecycle of its own, lifecycle of a component can be defined as the series of methods that are invoked in different stages of the component’s existence.

**Why do you sometimes need to “wrap” functions in useCallback when called from within useEffect**

useCallback will help in avoiding regeneration of functions when the functional component re-renders. However there isn't much of a performance difference caused by recreation of functions. You are specifying a function as a dependency to useEffect .

**Why are functional components preferred over class components?**

Functional component are much easier to read and test because they are plain JavaScript functions without state or lifecycle-hooks. You end up with less code. They help you to use best practices.

**What is wrong with the following code?**

`useEffect()` Location


```jsx
import React, {useState, useEffect} from 'react';

function MyComponent(props) {
  const [count, setCount] = useState(0);

  function changeCount(e) {
    setCount(e.target.value);
  }

  let renderedItems = []

  for (let i = 0; i < count; i++) {
    useEffect( () => {
      console.log('component mount/update');
    }, [count]);

    renderedItems.push(<div key={i}>Item</div>);
  }

  return (<div>
     <input type='number' value={count} onChange={changeCount}/>
      {renderedItems}
    </div>);
}
```


## Document the following Vocabulary Terms

|Term||
|---|---|
|state hook|The useState hook is a special function that takes the initial state as an argument and returns an array of two entries. Syntax: The first element is the initial state and the second one is a function that is used for updating the state. const [state, setState] = useState(initialstate)|
|effect hook|By using this Hook, you tell React that your component needs to do something after render. React will remember the function you passed (we'll refer to it as our “effect”), and call it later after performing the DOM updates.|
|reducer hook|useReducer is used to store and update states, just like the useState Hook. It accepts a reducer function as its first parameter and the initial state as the second.|




# Custom Hooks React
Custom Hooks are a mechanism to reuse stateful logic (such as setting up a subscription and remembering the current value), but every time you use a custom Hook, all state and effects inside of it are fully isolated. How does a custom Hook get isolated state? Each call to a Hook gets isolated state.

## Using a Custom Hook

Building your own Hooks lets you extract component logic into reusable functions.

When we were learning about using the Effect Hook, we saw this component from a chat application that displays a message indicating whether a friend is online or offline:

```jsx
import React, { useState, useEffect } from 'react';

function FriendStatus(props) {
  const [isOnline, setIsOnline] = useState(null);
  useEffect(() => {
    function handleStatusChange(status) {
      setIsOnline(status.isOnline);
    }
    ChatAPI.subscribeToFriendStatus(props.friend.id, handleStatusChange);
    return () => {
      ChatAPI.unsubscribeFromFriendStatus(props.friend.id, handleStatusChange);
    };
  });

  if (isOnline === null) {
    return 'Loading...';
  }
  return isOnline ? 'Online' : 'Offline';
}
```

Now let’s say that our chat application also has a contact list, and we want to render names of online users with a green color. We could copy and paste similar logic above into our FriendListItem component but it wouldn’t be ideal:

```jsx
import React, { useState, useEffect } from 'react';

function FriendListItem(props) {
  const [isOnline, setIsOnline] = useState(null);
  useEffect(() => {
    function handleStatusChange(status) {
      setIsOnline(status.isOnline);
    }
    ChatAPI.subscribeToFriendStatus(props.friend.id, handleStatusChange);
    return () => {
      ChatAPI.unsubscribeFromFriendStatus(props.friend.id, handleStatusChange);
    };
  });

  return (
    <li style={{ color: isOnline ? 'green' : 'black' }}>
      {props.friend.name}
    </li>
  );
}
```
Instead, we’d like to share this logic between FriendStatus and FriendListItem.

Traditionally in React, we’ve had two popular ways to share stateful logic between components: render props and higher-order components. We will now look at how Hooks solve many of the same problems without forcing you to add more components to the tree.



## Rules of Hooks
Only Call Hooks at the Top Level.
Only Call Hooks from React Functions.
Don’t call Hooks from regular JavaScript functions.


### 10 React Hooks you Should Have in Your Toolbox

1. useArray hook
1. react-use-form-state hook
1. react-fetch-hook
1. useMedia hook
1. react-useportal hook
1. react-firebase-hooks
1. use-onClickOutside hook
1. useIntersectionObserver hook
1. use-location hook
1. use-redux hook
