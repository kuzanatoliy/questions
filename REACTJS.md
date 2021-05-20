# ReactJS

## Links

### Questions

<details>
  <summary>What is React?</summary>

  React is Facebook's open-source JS library for building complex interactive UI in web and mobile applications. React's core purpose is building UI components. Generally, it is possible to use just the view in an MVC architecture.

</details>

<details>
  <summary>How does React work?</summary>

  React creates a virtual DOM. When state changes in a component, it firstly runs a "diffing" algorithm, which identifies what has changed in the virtual DOM. The second step is reconciliation, where it updates the DOM with the results of diff.

</details>

<details>
  <summary>What is Virtual DOM?</summary>

  The virtual DOM is an in-memory representation of Real DOM. React creates an in-memory data structure cache, computes the resulting differences, and then updates the browser's displayed DOM efficiently. It allows the programmer to write code as if the entire page is rendered on each change, while the React libraries only render subcomponents that change.

</details>

<details>
  <summary>What is JSX?</summary>

  JSX is a syntax extension to JavaScript and comes with the full power of JavaScript. JSX produces React "elements". You can embed any JS expression in JSX by wrapping it in curly braces. After compilation, JSX expressions become regular JavaScript objects.

</details>

<details>
  <summary>What is the difference between state and props?</summary>

  Both props and state are plain JavaScript objects. But they have different functionality.
  
  * The props get passed to the component similar to function parameters.
  
  * The React component can create the state object for the management of the inner state of it.

</details>

<details>
  <summary>What is a state in React?</summary>

  A state is similar to props, but it is private and fully controlled by the component. A state is necessarily an object that holds data and determines how the component renderers and behaves.

</details>

<details>
  <summary>What happens when you call setState?</summary>

  Firstly, when setState function called, React contacts a state and new state props, after that to start the agreement process that allows updating a view in one of the most effective ways. For it React generates a new tree of React elements and a comparison of new and old trees between themselves. It allows knowing what changes.

</details>

<details>
  <summary>What is the difference between element and component?</summary>

  Each React element is an object view of a user interface part.

  Each component is a function or class that gets data and returns a React element.

</details>

<details>
  <summary>When class components should be used without function components?</summary>

  It is possible to use class components if it has to work with state and life cycle methods. For all of the other cases, it is better to use the function component. One of the most important reasons to use a functional style is a minimization process. It is easier to minimize functions than classes.

  *Note*: Last versions of React allows using hooks for rendering optimization and state using.

</details>

<details>
  <summary>What are refs in React?</summary>

  A ref is an optional component's param that allows access to a DOM element or a component state. A value is a callback function that gets a link to the DOM element or the component as a first function argument.

  *Note:* It is bad practice to use ref. So, to use a callback mechanism for getting a child state property.

</details>

<details>
  <summary>What are the different phases of the React component lifecycle?</summary>

  There are four phases of React component's lifecycle:
  
  * Initialization: In this phase, a react component prepares settings up the initial state and default props.
  
  * Mounting: The react component is ready to mount in the browser DOM. This phase covers componentWillMount and componentDidMount lifecycle methods.
  
  * Updating: In this phase, the component gets updated in two ways, sending the new props and updating the state. This phase covers shouldComponentUpdate, componentWillUpdate and componentDidUpdate lifecycle methods.
  
  * Unmounting: In this last phase, the component is not needed and get unmounted from the browser DOM. This phase includes the componentWillUnmount lifecycle method.

</details>

<details>
  <summary>What are the keys to React? Why are they important?</summary>

  Keys are a unique identification of a component array. They are significant because the keys allow optimizing the rendering process. For example, without keys when the order in the component array, all elements would be rerendered. So keys allow being sure that rerender is needed.

</details>

<details>
  <summary>What is the render callback template?</summary>

  In this way, to use a callback function as a child component. So, children's props should be a function.

</details>

<details>
  <summary>What is the difference between stateful and stateless components?</summary>

  The stateful component has an inner state. Unlike, the stateless component does not have it.

</details>

<details>
  <summary>What method of the life cycle is better to use for calling an AJAX request?</summary>

  There are two lifecycle methods for AJAX requests.
  First and the best is componentDidMount.
  Second is componentWillMount. There are a few reasons why it is a bad idea:

  1. Firstly, there is not a conviction about when this method exactly would be called;
  2. There can be a situation when a request wouldn't resolve when a component tries to call setState or render a component.

</details>

<details>
  <summary>Why do you need to use shouldComponentUpdate?</summary>

  The shouldComponentUpdate allows controlling the compressing process of the current and his children when there is a conviction that the component had not had to be changed. So, for it, shouldComponentUpdate has to return false.

</details>

<details>
  <summary>How can you start to use production mode to React?</summary>

  Could be used to DefinePlugin for Webpack. It allows setting NODE_ENV in production. For example, in this case, there will be cat propType validation and other warnings.

</details>

<details>
  <summary>What are children?</summary>
  
  In JSX expressions that contain both an opening tag and a closing tag, the content between those tags is passed to the component automatically as a prop: 'props.children'.

</details>

<details>
  <summary>Why should you use Peact.Children.map without props.children.map?</summary>

  Because there is not a conviction that children prop will be an array.

</details>
