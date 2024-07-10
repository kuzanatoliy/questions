# CSS techniques

<details>
  <summary>What abjective of positioning content based on structural markup?</summary>

The objective of this technique is to demonstrate how visual appearance may be enhanced via style sheets while still maintaining a meaningful presentation when style sheets are not applied. Using the positioning properties of CSS, content may be displayed at any position on the user's viewport. Using structural elements that the meaning of the content can still be determined when styling is not available.

**Procedure:**

1. Remove the style information from the document or turn off use of style sheets in the user agent.
2. Check that the structural relations and the meaning of the content are preserved.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C6)

</details>

<details>
  <summary>What abjective of using CSS to hide a prtion of the link text?</summary>

The objective of this technique is to supplement the link text by adding additional text that describes the unique function of the link and styling the additional text so that is not rendered on the screen by user agents that support CSS. When information in the surrounding context is needed to interpret the displayed link text, this technique provides a complete description of the link's input function while permitting the less complete text to be displayed.

**Procedure:**

1. Check tat an element has been defined that confines its display to a pixel and hides the text.
2. Check that the element of that class is included in the content of the anchor.
3. Check that the combined content of the anchor describes the purpose of the link.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C7)

</details>

<details>
  <summary>What abjective of using CSS letter-spacing to control spacing within a work?</summary>

The objective of this technique is to demonstrate how the visual appearance of spacing in text may be enhanced via style sheets while still maintaning meaningful text sequencing. The CSS letter-spacing property helps developers control the amount of white space between characters. This is recommended over adding blank characters to control the spacing, since the blank characters can change the meaning and pronunciation of the word.

**Procedure:**

1. Check wheter the CSS letter-spacing property was used to control spacing.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C8)

</details>

<details>
  <summary>What abjective of using CSS to include decorative images?</summary>

The objective of this technique is to provide a mechanism to add purely decorative images and images used for visual formatting to Web content without requiring additional markup within the content. This makes it possible for assistive technologies to ignore the non-text content. Some user agents can ignore or turn off CSS at the user's request, so that background images included with CSS simply "disappear" and do not interfere with display settings such as enlarged fonts or high contrast settings.

**Procedure:**

1. Check for the presence of decorative images.
2. Check that they are included with CSS.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C9)

</details>

<details>
  <summary>What abjective of using percent for font sizes?</summary>

The objective of this technique is to specify text font size proportionally so that user agents can scale content effectively. If a font-size is specified for the body element, all other elements inherit that value, unless overriden by a more specific selector.

**Procedure:**

1. Check that the value of the CSS property that defines the font size is a percentage.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C12)

</details>
