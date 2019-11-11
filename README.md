# React-Render-Props
### Rendering props in React

### The main difference between state and props is that props are immutable. The container component should define the state that can be updated and changed, while the child components should only pass data from the state using props.

### You'll need immutable data in your component, so you can just add props to reactDOM.render() function in main.js and use it inside  the main component.
 
 ### In this example we set a default property values directly on the component constructor instead of adding it to the reactDom.render() element.
### We are using a class based component in this example, class based components are easier to maintain the state of app, they can also have lifecycle methods. Some of the lifecycle methods have been deprecated, here is an example (see next line)
 
 class App extends Component {

  UNSAFE_componentWillMount() {
    // ewwwww
  }

}

### This is a nudge to get all React developers to stop using these methods. (You must not use it)
### To allow easy renaming for projects where we may not have adequate time to migrate to the recommended lifecycle methods, the React team recommended a script from codemod that automates this process. (See next line)
cd your_project
npx
### We combined the state and props in the app. We are setting the state in our parent component and passing it down the component tree using props. Inside the render function, we are setting headerProp and contentProp used in child components. Hence the term passing props.

