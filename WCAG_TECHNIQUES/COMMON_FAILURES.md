# Common failures

<details>
  <summary>What is a failure of success criterion 1.3.2 due to changing the meaning of content by positioning information with CSS?</summary>

The describes the failure condition that results when CSS, rather than structural markup, is used to modify the visual layout of the content, and the modified layout changes the meaning of the content. Using the positioningproperties of CSS2, content may be displayed at any position on the user's viewport. The order in which items appear on a screen may be different than the order they are found in the source document. Assistive technologies rely on the source code or other programmatically determined order to render the content in the correct sequence. Thus, it is important not to rely on CSS to programmatically determined reading order.

**Procedure:**

1. Remove the style infromation from the document or turn off use of style sheets in the user agent.
2. Check that the reading order of the contnent is correct and the meaning of the content is preserved.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F1)

</details>
