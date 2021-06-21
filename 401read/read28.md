#  Component Composition


 ## Review, Research, and Discussion


**Can a parent component access the state of a child component?**

In React we can access the child’s state using Refs.  we will assign a Refs for the child component in the parent component. then using Refs we can access the child’s state.

Creating Refs Refs are created using React.createRef() and attached to React elements via the ref attribute.

**What can be passed along in a prop variable?**

Any type of data


**How can a child component “know” the state of another component?**

by pass it to the parent using props then read it 

### Document the following Vocabulary Terms
|Term||
|component props|Props are arguments passed into React components. Props are passed to components via HTML attributes.|
|component state|is an object that holds some information that may change over the lifetime of the component.|
|application state| is just a fancy term for a JavaScript data structure. If a user changes state by interacting with your application|

## **Preparation Materials**

### **react basics recap**
  1.  The Component Lifecycle

      ![](https://cdn-media-1.freecodecamp.org/images/1*U13Mlxz_ktcajaeJCyYkwg.png)

  2. Higher-Order Components

      A higher-order component is a function that takes a component and returns a new component.

  3. React State and setState()

     the State of a component is an object that holds some information that may change over the lifetime of the component.

     The only way you should change state is via the setState method. This method takes an object and merges it into the current state
  4. React Context

      The React context API allows you to create global context objects that can be given to any component you make. This allows you to share data without having to pass props down all the way through the DOM tree.


### **props.children**
   what `this.props.children` does is that it is used to display whatever you include between the opening and closing tags when invoking a component.
### **composition vs inheritance**

  - **Containment**

    **React** : Some components don’t know their children ahead of time. This is especially common for components like Sidebar or Dialog that represent generic “boxes”.

    We recommend that such components use the special children prop to pass children elements directly into their output.

  - **Specialization**

    Sometimes we think about components as being “special cases” of other components. For example, we might say that a WelcomeDialog is a special case of Dialog.

    In React, this is also achieved by composition, where a more “specific” component renders a more “generic” one and configures it with props

### <s>react testing library api example</s>
  
### **react-if component**

   -  Render React components conditionally.
   - Example: 
```js
      const Bar = ({ name, age, drinkingAge }) => (
  <div>
    <Header />
    <If condition={age >= drinkingAge}>
      <Then>
        <span className="ok">Have a beer, {name}!</span>
      </Then>
      <Else>
        <span className="not-ok">Sorry, {name}, you are not old enough.</span>
      </Else>
    </If>
    <Footer />
  </div>
);
```


### <s>react-testing-library-async</s>
