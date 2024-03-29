# Grid layout

### Links
[docs](https://css-tricks.com/snippets/css/complete-guide-grid/)

### Questions

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

  The space between two adjacent row and two adjacent column grid lines.

</details>

<details>
  <summary>What is a grid track?</summary>

  It is a space between two adjacent grid lines. You can think of them as the columns or rows of the grid.

</details>

<details>
  <summary>What is a grid area?</summary>

  It is a total space surrounded by four grid lines. A grid area may be composed of any number of grid cells.

</details>

<details>
  <summary>How can be set an element as a grid container?</summary>

  Need to set a `display` css property of an element to `grid` or `inline-grid` values.

</details>

<details>
  <summary>How can be set a count of columns and rows of the grid component?</summary>

  This bihaviour could be controlled by `grid-template-columns` and `grid-template-rows` css properties. For example, grid-template-columns: `[line1] 50% [line2] 50%`. Moreover, possible to combine these properties using grid-template property. For example, `<grid-template-rows> / <grid-template-columns>`

</details>

<details>
  <summary>How can be worked with the grid areas?</summary>

  Could be controlled by a `gird-template-areas` property, It allows to use a map of areas. In this case, each grid element should have a name that was set by a `grid-area` property.

</details>

<details>
  <summary>Is it possible adding space between grid cells?</summary>

  Could be set gaps between columns by the `grid-column-gap` or the `column-gap`. And could be set gaps between rows by the `grid-row-gap` or the `row-gap`. For example, `gap: <row-gap> <column-gap>`

</details>

<details>
  <summary>How can be aligned the content of each grid cells?</summary>

  Could be aligned by the `justify-items` property in rows and could be aligned by the `align-items` in columns. Possible to use values: `start`, `end`, `center` or `stretch`. Moreover, the properties have a combination with the `place-items` property. For example, place-items: `<justify-items> <align-items>`. Besides, each grid element can be aligned with only one element using identical settings (`justify-self` / `align-self` / `place-self`).

</details>

<details>
  <summary>How can be aligned with the grid component?</summary>

  Could be aligned by the `justify-content` in rows or by the `align-content` in columns. Could be set values: `start`, `end`, `center`, `stretch`, `space-around`, `space-between` or `space-evenly`. Also, it's possible for combining these settings using `place-items`. For example, `place-content: <justify-content> <align-content>`

</details>

<details>
  <summary>Is it possible adding the size of the grid cells?</summary>

  Could be managed by the `gird-auto-columns` and `grid-auto-rows` properties.

</details>

<details>
  <summary>How can be added to the auto-placement algorithm?</summary>

  Could be managed by the `grid-auto-flow` (`row`, `column`, `row dense`, `column dense`).

</details>

<details>
  <summary>How can be set the grid area for grid element?</summary>

  Could be managed by the properties: `grid-column-start` / `grid-column-end` / `grid-row-start` / `grid-row-end` or combining `grid-column` / `grid-row`

</details>
