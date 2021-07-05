# Readings: Redux - Asynchronous Actions



**How granular should your reducers be?**

full-warp with very specific events, dedicated for every change

**Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched**

pro


**Name a strategy for preventing the above**

combine reducers



|Term||
|----|----|
|store|A store is an immutable object tree in Redux. A store is a state container which holds the application's state. Redux can have only a single store in your application.|
|combined reducers|The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore .|


## Async Logic and Data Fetching

### Redux Middleware and Side Effects

By itself, a Redux store doesn't know anything about async logic. It only knows how to synchronously dispatch actions, update the state by calling the root reducer function, and notify the UI that something has changed. Any synchronicity has to happen outside the store.

![](https://redux.js.org/assets/images/ReduxAsyncDataFlowDiagram-d97ff38a0f4da0f327163170ccc13e80.gif)

Earlier, we said that Redux reducers must never contain "side effects". A "side effect" is any change to state or behavior that can be seen outside of returning a value from a function. Some common kinds of side effects are things like:

- Logging a value to the console
- Saving a file
- Setting an async timer
- Making an AJAX HTTP request
- Modifying some state that exists outside of a function, or mutating arguments to a function
- Generating random numbers or unique random IDs (such as Math.random() or Date.now())



## Using the Redux Thunk Middleware

**Configuring the Store**

The Redux thunk middleware is available on NPM as a package called redux-thunk. We need to install that package to use it in our app:

```
npm install redux-thunk
```

Once it's installed, we can update the Redux store in our todo app to use that middleware:

```jsx
import { createStore, applyMiddleware } from 'redux'
import thunkMiddleware from 'redux-thunk'
import { composeWithDevTools } from 'redux-devtools-extension'
import rootReducer from './reducer'

const composedEnhancer = composeWithDevTools(applyMiddleware(thunkMiddleware))

// The store now has the ability to accept thunk functions in `dispatch`
const store = createStore(rootReducer, composedEnhancer)
export default store
```