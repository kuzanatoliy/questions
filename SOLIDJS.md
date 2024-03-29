# SolidJS

<details>
  <summary>What is SolidJS?</summary>

Solid is a JavaScript framework for making interactive web applications in a declarative style (it links data and classes that it uses and creates). Also it allows to use JSX, that allows using existing HTML and JavaScript knowledge to build components that can be reused throughout your app.

[More >>](https://www.solidjs.com/tutorial/introduction_basics)

</details>

<details>
  <summary>What is a JSX?</summary>

JSX is HTML-like syntax that can be used for building components. JSX adds dynamic expressions that allow you to reference variables and functions within your HTML by using the { } syntax.

It is possible to mention three main differences between JSX and HTML that prevent JSX from being seen as a superset of HTML:


* JSX does not have void elements. This means that all elements must have a closing tag or self-close;
* JSX must return a single Element;
* JSX does not support the HTML Comments.

[More >>](https://www.solidjs.com/tutorial/introduction_jsx)

</details>

<details>
  <summary>What is a Component?</summary>

Components are functions that typically return JSX and other components can call them by JSX in other components.

[More >>](https://www.solidjs.com/tutorial/introduction_components)

</details>

<details>
  <summary>What are Signals?</summary>

Signals are the cornerstone of reactivity in Solid. They contain values that change over time; when you change a signal's value, it automatically updates anything that uses it. It is needed to use ``createSignal`` function for creating the Signal.

[More >>](https://www.solidjs.com/tutorial/introduction_signals)

</details>

<details>
  <summary>What is an Effect?</summary>

An Effect is an observer that allows running side-effects that have dependencies from signals. It is possible to use ``createEffect`` or ``createRenderEffect``.

[More >>](https://www.solidjs.com/tutorial/introduction_effects)

</details>

<details>
  <summary>What are drived Signals?</summary>

A function that accesses a signal is effectively also a signal: when its wrapped signal changes, it will in turn update its readers.

[More >>](https://www.solidjs.com/tutorial/introduction_derived)

</details>

<details>
  <summary>What are Memos?</summary>

Memos are both an observer, like an effect, and a read-only signal. Since they are aware of both their dependencies and observers, they can ensure that they run only once for any change.

[More >>](https://www.solidjs.com/tutorial/introduction_memos)

</details>

<details>
  <summary>Is it possible to use conditions in component?</summary>

1. Ternary operations ``a ? componentA : componentB``;
2. Boolean expressions ``a && componentA``;
3. Show component.

[More >>](https://www.solidjs.com/tutorial/flow_show)

</details>

<details>
  <summary>What is a For component?</summary>

The ``For`` component is a way to loop over an array of objects. As the array changes, ``For`` updates or moves items in the DOM rather than recreating them. The component has ``each`` property where it is possible to pass an array and get a callback (the same as for a map). 

**Note:** an index is signal.

[More >>](https://www.solidjs.com/tutorial/flow_for)

</details>

<details>
  <summary>What is an Index component?</summary>

The ``Index`` component is a way to loop over an array of objects, which will cause less rerenders in certain situations. It has a similar signature to ``For``, except this time, the item is the signal, and the index is fixed.

**Note:** a value is signal.

[More >>](https://www.solidjs.com/tutorial/flow_index)

</details>

<details>
  <summary>What is a Switch?</summary>

Sometimes it is needed to deal with conditionals with more than 2 mutual exclusive outcomes. For this case, we have the ``Switch`` and ``Match`` components modeled roughly after JavaScript's switch/case.

[More >>](https://www.solidjs.com/tutorial/flow_switch)

</details>

<details>
  <summary>What is a Dynamic?</summary>

The ``Dynamic`` tag is useful when you render from data. It lets you pass either a string for a native element or a component function and it will render that with the rest of the provided props.

[More >>](https://www.solidjs.com/tutorial/flow_dynamic)

</details>

<details>
  <summary>What is a Portal?</summary>

The ``Portal`` component allows inserting content at the location of your choosing. By default, its elements will be rendered in a ``div`` in the ``document.body``.

[More >>](https://www.solidjs.com/tutorial/flow_portal)

</details>

<details>
  <summary>What is an ErrorBoundary?</summary>

A JavaScript error originating in the UI should not break the entire app. Error boundaries are components that catch JavaScript errors anywhere in their child component tree, log those errors, and display a fallback UI instead of the component tree that crashed.

[More >>](https://www.solidjs.com/tutorial/flow_error_boundary)

</details>

<details>
  <summary>What are life-cycle methods?</summary>

**onMount** is just a createEffect call that is non-tracking, which means it never re-runs. It is just an Effect call but it is possible to use it with confidence that it will run only once for your component, once all initial rendering is done.

[More >>](https://www.solidjs.com/tutorial/lifecycles_onmount)

**onCleanup**. It is possible to call it at any scope and it will run when that scope is triggered to re-evaluate and when it is finally disposed.

[More >>](https://www.solidjs.com/tutorial/lifecycles_oncleanup)

</details>

<details>
  <summary>How is it possible to handle events?</summary>

1. Solid supports an array syntax to call the handler with data (as the first argument) without creating additional closures:

    const handler = (data, event) => /*...*/

    <button onClick={[handler, data]}>Click Me</button>

2. It is possible to pass only hanlder:

    <div onMouseMove={handleMouseMove}>
      The mouse position is {pos().x} x {pos().y}
    </div>

3. If it is needed to support other casings or not use event delegation, you can use ``on:`` namespace to match event handlers:

    <button on:DOMContentLoaded={() => /* Do something */} >Click Me</button>

[More >>](https://www.solidjs.com/tutorial/bindings_events)

</details>

<details>
  <summary>How is it possible to set up style?</summary>

The style attribute in Solid accepts either style strings or objects. However the object form differs from Element.prototype.style and instead is a wrapper for calling style.setProperty. This means that keys take the dash-case form, such as ``background-color`` rather than ``backgroundColor``, and that any units must be explicitly provided (e.g., ``width: 500px`` rather than ``width: 500``).

[More >>](https://www.solidjs.com/tutorial/bindings_style)

</details>

<details>
  <summary>How is it possible to set up class?</summary>

Solid uses ``class`` to set the className property on an element. However, it is often convenient to conditionally set classes. For that reason, Solid has a built-in ``classList`` JSX attribute that takes an object where the key is the class name(s) and the value is a boolean expression. When true, the class is applied, and when false, it is removed.

[More >>](https://www.solidjs.com/tutorial/bindings_classlist)

</details>

<details>
  <summary>How is it possible to access to DOM element?</summary>

Refs are basically assignments, which happen at creation time before they are attached to the document DOM. Just declare a variable, pass it in as a ref attribute, and the variable will be assigned.

**Note:** it is possible to forwrd refs through props.

[More >>](https://www.solidjs.com/tutorial/bindings_refs)

</details>

<details>
  <summary>How is it possible to pass a variable number of attributes?</summary>

Sometimes your components and elements accept a variable number of attributes and it makes sense to pass them down as an object instead of individually. So, It is possible to use a spred operator.

**Note:** it is possible to forwrd refs through props.

[More >>](https://www.solidjs.com/tutorial/bindings_refs)

</details>

<details>
  <summary>What is a derective?</summary>

This is just a syntactic sugar over ref, but is useful in that it resembles typical bindings and there can be multiple bindings on the same element without conflict. This makes it a better tool for reusable DOM element behavior.

**Note:** It is possible to set up a derective by ``use:`` namespace.

[More >>](https://www.solidjs.com/tutorial/bindings_directives)

</details>

<details>
  <summary>How is it possible to set up default props to a component?</summary>

It is possibel to use ``mergeProps``, which merges potentially reactive objects together (like a nondestructive ``Object.assign``) without losing reactivity. The most common case is when setting default props components.

[More >>](https://www.solidjs.com/tutorial/props_defaults)

</details>

<details>
  <summary>How is it possible to split props?</summary>

For this purpose, Solid has ``splitProps``. It takes the props object and one or more arrays of keys that we want to extract into their own props objects. It returns an array of props objects, one per array of specified keys, plus one props object with any remaining keys. All returned objects preserve reactivity.

[More >>](https://www.solidjs.com/tutorial/props_split)

</details>

<details>
  <summary>Is it correct to work with a children directly?</summary>

No. For that reason, Solid has the ``children`` helper. This method both creates a memo around the ``children`` prop and resolves any nested child reactive references so that you can interact with the children directly.

[More >>](https://www.solidjs.com/tutorial/props_children)

</details>

<details>
  <summary>How is it possible to create a store? What is a store?</summary>

The ``createStore`` call takes the initial value and returns a read/write tuple similar to Signals. The first element is the store proxy which is readonly, and the second is a setter function.

The setter function in its most basic form takes an object whose properties will be merged with the current state. It also supports path syntax so that we can do nested updates. In this way we can still maintain control of our reactivity but do pinpoint updates.

[More >>](https://www.solidjs.com/tutorial/stores_createstore)

</details>

<details>
  <summary>Is it possible to make mutation to store?</summary>

Yes. It is possible to use ``produce`` function or to create mutable store by ``createMutable``. However, it is not recomended.

[More >>](https://www.solidjs.com/tutorial/stores_mutation)

</details>

<details>
  <summary>Is it possible to pass data around without relying on passing through props?</summary>

Solid provides a Context API to pass data around without relying on passing through props. This is useful for sharing Signals and Stores. Using Context has the benefit of being created as part of the reactive system and managed by it. Context is also useful when have a need to "override" your state in a certains part of the component tree.

[More >>](https://www.solidjs.com/tutorial/stores_context)

</details>

<details>
  <summary>Is it possible to use immutable stores as redux?</summary>

Yes. However, it is needed to use ``reconcile`` method that enhances the setStore call and lets us diff the data from these immutable sources, only notifying the granular updates.

[More >>](https://www.solidjs.com/tutorial/stores_immutable)

</details>

<details>
  <summary>What are batching updates?</summary>

Solid's ``batch`` helper allows to queue up multiple changes and then apply them all at the same time before notifying their observers.

[More >>](https://www.solidjs.com/tutorial/reactivity_batch)

</details>

<details>
  <summary>What is an untrack helper?</summary>

Solid provides the ``untrack`` helper as a way to prevent the wrapping computation from tracking any reads.

[More >>](https://www.solidjs.com/tutorial/reactivity_untrack)

</details>

<details>
  <summary>What is an on helper?</summary>

Solid has an ``on`` helper that enables setting explicit dependencies for our computations. This is mostly used as a terse way to be even more explicit about which Signals are tracked (and not track any other Signals, even if they are read).

[More >>](https://www.solidjs.com/tutorial/reactivity_on?solved)

</details>

<details>
  <summary>Is it possible to use dinamic imports?</summary>

Solid's lazy method allows us to wrap the component's dynamic import for deferred lazy loading. The output is a Component that can be used as normal in our JSX template with the exception that internally it dynamically loads the underlying imported code when it is rendered the first time, halting that branch of rendering until the code is available.

[More >>](https://www.solidjs.com/tutorial/async_lazy)

</details>

<details>
  <summary>What is possible to use for async loading?</summary>

It is possible to use ``createResource`` signal for handling async loading. Resources are special Signals designed specifically to handle Async loading. Their purpose is to wrap async values in a way that makes them easy to interact with in Solid's distributed execution model.

[More >>](https://www.solidjs.com/tutorial/async_resources)

</details>

<details>
  <summary>What is a Suspense component?</summary>

``Suspense`` serves as a boundary that can show a fallback placeholder instead of the partially loaded content as these async events resolve. Moreover, it is possible to use ``SuspenseList`` component for combining a few cases.

It is possible to avoid going back to the fallback state by leveraging ``useTransition``. It provides a wrapper and a pending indicator. The wrapper puts all downstream updates in a transaction that doesn't commit until all async events complete.

[More >>](https://www.solidjs.com/tutorial/async_suspense)

</details>
