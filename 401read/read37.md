# Readings: Redux - Combined Reducers

## Review, Research, and Discussion


**Why choose Redux instead of the Context API for global state?**

**Context API** is easy to is use as it has a short learning curve. It requires less code, and because there's no need of extra libraries, bundle sizes are reduced. **Redux** on the other hand requires adding more libraries to the application bundle. The syntax is complex and extensive creating unnecessary work and complexity.

**What is the purpose of a reducer?**

In Redux, a reducer is a pure function that takes an action and the previous state of the application and returns the new state. The action describes what happened and it is the reducer's job to return the new state based on that action. It may seem simple, but it does have to be a pure function with no side effects


**What does an action contain?**

Actions are the only source of information for the store as per Redux official documentation. It carries a payload of information from your application to store. const ITEMS_REQUEST = 'ITEMS_REQUEST'; Apart from this type attribute, the structure of an action object is totally up to the developer.


**Why do we need to copy the state in a reducer?**

Reducers specify how the application's state changes in response to actions sent to the store. Remember that actions only describe what happened, but don't describe how the application's state changes. So whenever you call an action, reducer must return a new state based on that action.





|Term||
|---|---|
|immutable state|Immutable data updates means that new object references are created, and thus connect will see that the data has changed and the UI needs to update|
|time travel in redux|Time travel is the ability to move back and forth among the previous states of an application and view the results in real time. With Redux, given a specific state and a specific action, the next state of the application is always exactly the same.|
|action creator|An action creator is merely a function that returns an action object. Redux includes a utility function called bindActionCreators for binding one or more action creators to the store's dispatch() function.|
|reducer|In Redux, a reducer is a pure function that takes an action and the previous state of the application and returns the new state. The action describes what happened and it is the reducer's job to return the new state based on that action.|
|dispatch|dispatch is a function of the Redux store. You call store. dispatch to dispatch an action. This is the only way to trigger a state change. With React Redux, your components never access the store directly - connect does it for you.|


## `combineReducers(reducers)`


The `combineReducers` helper function turns an object whose values are different reducing functions into a single reducing function you can pass to `createStore`.

The resulting reducer calls every child reducer, and gathers their results into a single state object. The state produced by` combineReducers()` namespaces the states of each reducer under their keys as passed to `combineReducers()`

**Example :**

```js

rootReducer = combineReducers({potato: potatoReducer, tomato: tomatoReducer})
// This would produce the following state object
{
  potato: {
    // ... potatoes, and other state managed by the potatoReducer ...
  },
  tomato: {
    // ... tomatoes, and other state managed by the tomatoReducer, maybe some nice sauce? ...
  }
}

```



