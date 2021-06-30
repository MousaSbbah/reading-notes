# `<Login />` and `<Auth />`




## Review, Research, and Discussion


**Why is the Context API useful?**

The React Context API is a way for a React app to effectively produce global variables that can be passed around.

**Can a component outside of a provider get its context?**

No

**What are some common use cases for using the Context API?**

Theming  --- setting





## Document the following Vocabulary Terms
|Term||
|----|-----|
|global state|Context provides a way to pass data through the component tree without having to pass props down manually at every level, managing state in multiple components that are not directly connected.|
|global context|share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language. |
|provider|component that allows consuming components to subscribe to context changes|
|consumer|A React component that subscribes to context changes. Using this component lets you subscribe to a context within a function component.|



## DEFINITION OF ROLE-BASED ACCESS CONTROL (RBAC)
Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.

Employees are only allowed to access the information necessary to effectively perform their job duties. Access can be based on several factors, such as authority, responsibility, and job competency. In addition, access to computer resources can be limited to specific tasks such as the ability to view, create, or modify a file.

## Cookies

 are the data stored in the form of key-value pairs that are used to store information about the user on their computer by the websites that the users browse and use it to verify them.

 ## React-cookie component (Usage)

 ```jsx

import { Component } from 'react'
import cookie from 'react-cookies'
 
import LoginPanel from './LoginPanel'
import Dashboard from './Dashboard'
 
class MyApp extends Component {
  constructor () {
    super()
 
    this.onLogin = this.onLogin.bind(this)
    this.onLogout = this.onLogout.bind(this)
  }
 
  componentWillMount() {
    this.state =  { userId: cookie.load('userId') }
  }
 
  onLogin(userId) {
    this.setState({ userId })
    cookie.save('userId', userId, { path: '/' })
  }
 
  onLogout() {
    cookie.remove('userId', { path: '/' })
  }
 
  render() {
    const { userId } = this.state
 
    if (!userId) {
      return <LoginPanel onSuccess={this.onLogin} />
    }
 
    return <Dashboard userId={userId} />
  }
}

```

