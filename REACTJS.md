# ReactJS

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

  Class components are used if it has to work with state and life cycle methods. For all of the other cases have to be used function components. One of the most important reasons to use a functional style is a minimization process. It is easier to minimize functions then classes.
  *Note*: Last versions of the React allows using hooks for a rendering optimization and a state using.

</details>

<details>
  <summary>What are refs in React?</summary>

  A ref is an optional component's param that allows access to a DOM element or a component state. A value is a callback function that gets a link to the DOM element or the component as a first function argument.
  *Note:* It is bad practice to use ref. So, to use a callback mechanism for getting a child state property.

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
  <summary>What method of the life cycle should be used to call an AJAX request?</summary>

  There are two lifecycle methods for AJAX requests.
  First and the best is componentDidMount.
  Second is componentWillMount. There are a few reasons why it is a bad idea:
  1. Firstly, there is not a conviction about when this method exactly would be called;
  2. There can be a situation when a request wouldn't resolve when a component tries to call setState or render a component.


</details>

<details>
  <summary>Why shouldComponentUpdate is an important life cycle method?</summary>

  ...in progress

</details>

<details>
  <summary>How you can start to use production mode to React?</summary>

  ...in progress

</details>

<details>
  <summary>Why should you use Peact.Children.map without props.children.map?</summary>

  ...in progress

</details>
