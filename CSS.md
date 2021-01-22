# CSS

# CSS Grid layout

<details>
  <summary>What is a grid container?</summary>

  Grid container is applied by 'display: grid’ property. All children elements align in lines and columns.

</details>

<details>
  <summary>What is a grid item?</summary>

  A grid item is any child element of a grid container.

</details>

<details>
  <summary>What is a grid line?</summary>

  A grid line is each line that makes up the structure of the grid. It can be either vertical (column grid lines) or horizontal (row grid lines) and reside on either side of a row or column.

</details>

<details>
  <summary>What is a grid cell?</summary>

  In progress ...

</details>

<details>
  <summary>What is a grid track?</summary>

  In progress ...

</details>

<details>
  <summary>What is a grid area?</summary>

  In progress ...

</details>

<details>
  <summary>How can be set an element as a grid container?</summary>

  In progress ...

</details>

<details>
  <summary>How can be set a count of columns and rows of the grid component?</summary>

  In progress ...

</details>

<details>
  <summary>How can be worked with the grid areas?</summary>

  In progress ...

</details>

<details>
  <summary>Is it possible adding space between grid cells?</summary>

  In progress ...

</details>

<details>
  <summary>How can be aligned the content of each grid cells?</summary>

  In progress ...

</details>

<details>
  <summary>How can be aligned with the grid component?</summary>

  In progress ...

</details>

<details>
  <summary>Is it possible adding the size of the grid cells?</summary>

  In progress ...

</details>

<details>
  <summary>How can be added to the auto-placement algorithm?</summary>

  In progress ...

</details>

<details>
  <summary>How can be set the grid area for grid element?</summary>

  In progress ...

</details>

### CSS Flexbox layout

<details>
  <summary>What does flexbox technology based?</summary>

  Each of the flexbox containers has the base and secondary axis directed perpendicularly each other. Flexbox items suited on the base axis can be moved or stretched out by the secondary axis.

</details>

<details>
  <summary>How can be used Flexbox on an HTML page?</summary>

  Need to set a `display` css property of elemtn to `flex` or `inline-flex` values.

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
