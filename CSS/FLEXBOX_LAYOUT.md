# Flexbox layout

### Links
[docs](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

## Questions

<details>
  <summary>What does flexbox technology based?</summary>

  Each of the flexbox containers has the base and secondary axis directed perpendicularly each other. Flexbox items suited on the base axis can be moved or stretched out by the secondary axis.

</details>

<details>
  <summary>How can be used Flexbox on an HTML page?</summary>

  Need to set a `display` css property of an element to `flex` or `inline-flex` values.

</details>

<details>
  <summary>How can be changed the direction of container axes?</summary>

  The direction of flexbox elements could be managed by `flex-direction` property into a flexbox container element. There are the next available values: `row`, `column`, `row-reverse`, `column-reverse`.

</details>

<details>
  <summary>Does Flexbox allow wrapping elements?</summary>

  A base flexbox elements behaviour is fitting elements onto one line. This behaviour can be changed by wrap property for a flexbox container. There are the next available values: `nowrap`, `wrap`, `wrap-reverse`. Moreover, possible to combine `flex-direction` and `flex-wrap` by `flex-flow` property.

</details>

<details>
  <summary>How can elements be aligned?</summary>

  Flexbox elements can be aligned by `justify-content`(the base axis) and `align-content`(the secondary axis). There are the next available properties: `flex-start`, `flex-end`, `center`, `space-between`, `space-around`. Moreover, it’s possible managing how flex items laid out along the secondary axis on the current line. There are the next available properties: `stretch`, `flex-start`, `flex-end`, `center`, `baseline`. Besides, item align could be managed for only one element by `align-self` property.

</details>

<details>
  <summary>Can an order of Flexbox elements be changed?</summary>

  Order one of the flexbox elements can change by `order` property.

</details>

<details>
  <summary>Can the size of a Flexbox element be managed?</summary>

  The `flex-grow` property defines the ability for a flex item to grow if necessary. It accepts a unitless value that serves as a proportion. It dictates what amount of the available space inside the flex container the item should take up.
  
  The `flex-shrink` property defines the ability for a flex item to shrink if necessary.
  
  The `flex-basis` property defines the default size of an element before the distribution of the remaining space.
  Moreover, there can use a combination of these properties in `flex` property.

</details>
