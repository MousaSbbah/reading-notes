# Redux - Additional Topics

## Review, Research, and Discussion

- **What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?**
  The most 'redux-like' way of handling the pre-loading of data would be to fire off the asynchronous action in the lifecycle method (probably componentWillMount ) of a Higher Order Component that wraps your app.
- **When using a thunk/async action that dispatches the actual action, which do you export from your reducer?**

  - by default : export the reducer
  - for the dispatch function : export function which return async function which return a dispatch

## Document the following Vocabulary Terms

| Term       |     |
| ---------- | --- |
| middleware |     |
| thunk      |     |


# Redux Toolkit

## What is Redux Toolkit?#
Redux Toolkit is our official, opinionated, batteries-included toolset for efficient Redux development. It is intended to be the standard way to write Redux logic, and we strongly recommend that you use it.

It includes several utility functions that simplify the most common Redux use cases, including store setup, defining reducers, immutable update logic, and even creating entire "slices" of state at once without writing any action creators or action types by hand. It also includes the most widely used Redux addons, like Redux Thunk for async logic and Reselect for writing selector functions, so that you can use them right away.


## What's Included

- `configureStore()`: wraps createStore to provide simplified configuration options and good defaults. it can automatically combine your slice reducers, adds whatever Redux middleware you supply, includes redux-thunk by default, and enables use of the Redux DevTools Extension.


- `createReducer()`: that lets you supply a lookup table of action types to case reducer functions, rather than writing switch statements. In addition, it automatically uses the immer library to let you write simpler immutable updates with normal mutative code, like state.


- `createAction()`: generates an action creator function for the given action type string. The function itself has toString() defined, so that it can be used in place of the type constant.


- `createSlice()`: accepts an object of reducer functions, a slice name, and an initial state value, and automatically generates a slice reducer with corresponding action creators and action types.


- `createAsyncThunk`: accepts an action type string and a function that returns a promise, and generates a thunk that dispatches pending/fulfilled/rejected action types based on that promise
createEntityAdapter: generates a set of reusable reducers and selectors to manage normalized data in the store


- The   `createSelector` utility from the Reselect library, re-exported for ease of use.







# MobX

## Introduction
Anything that can be derived from the application state, should be. Automatically.

MobX is a battle tested library that makes state management simple and scalable by transparently applying functional reactive programming (TFRP). The philosophy behind MobX is simple:

- **Straightforward**
Write minimalistic, boilerplate free code that captures your intent. Trying to update a record field? Use the good old JavaScript assignment. Updating data in an asynchronous process? No special tools are required, the reactivity system will detect all your changes and propagate them out to where they are being used.

- **Effortless optimal rendering**
All changes to and uses of your data are tracked at runtime, building a dependency tree that captures all relations between state and output. This guarantees that computations depending on your state, like React components, run only when strictly needed. There is no need to manually optimize components with error-prone and sub-optimal techniques like memoization and selectors.

- **Architectural freedom**
MobX is unopinionated and allows you to manage your application state outside of any UI framework. This makes your code decoupled, portable, and above all, easily testable.


## example
So what does code that uses MobX look like?
```jsx
import React from "react"
import ReactDOM from "react-dom"
import { makeAutoObservable } from "mobx"
import { observer } from "mobx-react"

// Model the application state.
class Timer {
    secondsPassed = 0

    constructor() {
        makeAutoObservable(this)
    }

    increase() {
        this.secondsPassed += 1
    }

    reset() {
        this.secondsPassed = 0
    }
}

const myTimer = new Timer()

// Build a "user interface" that uses the observable state.
const TimerView = observer(({ timer }) => (
    <button onClick={() => timer.reset()}>Seconds passed: {timer.secondsPassed}</button>
))

ReactDOM.render(<TimerView timer={myTimer} />, document.body)

// Update the 'Seconds passed: X' text every second.
setInterval(() => {
    myTimer.increase()
}, 1000)

```

![](https://mobx.js.org/assets/flow2.png)




# HookState

Hookstate is a modern alternative to Redux, Mobx, Recoil, etc. It is simple to learn, easy to use, extendable, very flexible and capable to address all state management needs of large scalable applications. It has got impressive performance and predictable behavior.


