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

  Can be used class component if it has to work with a state or a life cycle methods. For all of the other cases have to be used function components.  One of the most important reasons to use a functional style is a minimization process. It is easier to minimize functions then classes.
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

  ...in progress

</details>

<details>
  <summary>What is the difference between stateful and stateless components?</summary>

  ...in progress

</details>

<details>
  <summary>What method of the life cycle should be used to call an AJAX request?</summary>

  ...in progress

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
