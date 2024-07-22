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

<details>
  <summary>What abjective of using named font sizes?</summary>

The objective of this technique is to specify a named font size that expresses the relative font size desired. These values provide hints so taht the user agent can choose a font-size relative to the inherited font-size.

**Procedure:**

1. Check that the value of the CSS property that defines the font size is one of xx-small, x-small, small, medium, large, x-large, xx-large, smaller, or larger.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C13)

</details>

<details>
  <summary>What abjective of using em units for font sizes?</summary>

The objective of this technique is to specify text font size in em units so that user agents can scale content effectively. Since the em is a property of the font, it scales as the font changes size. If a font-size is specified for the body element, all other elements inherit that value, unless overridden by a more specific selector.

**Procedure:**

1. Check that the value of the CSS property that defines the font size is expressed in em units.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C14)

</details>

<details>
  <summary>What abjective of using CSS to change the presentation of a user interface component when it receives focus?</summary>

The objective of this technique is to demonstrate how visual appearance may be enhanced via style sheets to provide visual feedback when an interactive element has focus or when a user hovers over it using a pointing device.

**Procedure:**

1. Using a keyboard, tab to he component.
2. Check that the focus indicator changes color.
3. Check that the focus indicator is removed when the component loses focus.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C15)

</details>

<details>
  <summary>What abjective of scaling form elements which contain text?</summary>

The objective of this technique is to ehsure text-based form controls resize when text size is changed in the user agent. This will allow users to enter text and read what they have entered in input boxes because the text is displayed at the size required by the user.

**Procedure:**

1. Enter some text into text based form controls that receive user entered text.
2. Increase the text size of the content by 200%.
3. Check that the text in text based form controls has increased by 200%.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C17)

</details>

<details>
  <summary>What abjective of using CSS margin and padding rules instead of spacer images for layout design?</summary>

Web designers sometimes use spacer images (usually 1x1 pixel, transparent GIFs) for better control over layout, for example in tables or to indent a paragraph. However, Cascading Style Sheets (CSS) allow sufficient control over layout to replace spacer images.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C18)

</details>

<details>
  <summary>What abjective of specifying alignment either to the left or right in CSS?</summary>

This technique describes how to align blocks of text either left or right by setting the CSS text-align property.

**Procedure:**

1. Check that the text is aligned either left or right.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C19)

</details>

<details>
  <summary>What abjective of using relative measurements to set column widths so that lines can average 80 characters or less when the browser is resized?</summary>

The purpose of this technique is to ensure that CSS is used in a way tat allows users to view content in such a way that line length can average 80 characters or less. This makes it possible for users with certain reading or vision disabilities that have trouble keeping their place when reading long lines of text to view and interact with the content more efficiently. This technique also allows for column width to grow wider as font sizes increase, which will reduce the possibility of clipping as the text size increases.

**Procedure:**

1. Test to see that the coluns are defined in relative units.
2. Check to see that line length can be set to 80 characters or less by resizing the browser window.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C20)

</details>

<details>
  <summary>What abjective of specifying line spacing in CSS?</summary>

Many people with cognitive disabilities have trouble tracking lines of text when a block of text is single spaced. Providing spacing between 1.5 to 2 allows them to start a new line more easily once they have finished the previous one.

**Procedure:**

1. Open content in a browser.
2. Check that the spacing between lines in blocks of text is between 1.5 and 2.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C21)

</details>

<details>
  <summary>What abjective of using CSS to control visual presentation of text?</summary>

The objective of this technique is to demonstrate how CSS can be used to control the visuaal presentation of text. This will allow users to modify, via the user agent, the visual characteristics of the text to meet their requirement. The text characteristics include aspects such as size, color, font family and relative placement.

**Procedure:**

1. Check whether CSS properties were used to control the visual presentation of text.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C22)

</details>

<details>
  <summary>What abjective of specifying text and background colors of secondary content such as banners, features and navigation in CSS while not specifying text and background colors of the main content?</summary>

Some Web pages use colors to identify different groupings. The objective of this technique is to allow users to select specific color combinations for the text and background of the main content while retaning visual clues to the groupings and organization of the web page. When a user overrides the foreground colors of all the text on a page, visual clues to the grouping and organization of the Web page may be lost, making it much more difficult to understand and use.

**Procedure:**

1. Change the text, link and background colors in the browser settings so they are different from the default color and different from those specified in the secondary content.
2. Check that the main content uses the new text, link and background colors.
3. Check that the colors of the text, links and backgrounds in the secondary content has not changed.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C23)

</details>

<details>
  <summary>What abjective of using percentage values in CSS for container sizes?</summary>

The objective of this technique is to enable users to increase the size of text without having to scroll horizontally to read that text. To use this technique, an author specifies the width of text containers using percent values.

**Procedure:**

1. Check that all container widths are specified as percentage values.
2. Increase the text size to 200%.
3. Check to make sure that horizontal scrolling is not required to read any line of text.
4. Check that all text is still visible on the page.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C24)

</details>

<details>
  <summary>What abjective of specifying borders and layout in CSS to delineate areas of a Web page while not specifying text and text-background colors?</summary>

The intent of this technique is to specify boders and layout using CSS and leave text and background colors to render according to the user's browser and/or operating system settings. This allows users to view the text in the colors they require while maintaining other aspects of the layout and page design such as columns of text, borders around sections or vertical lines between a menu and main content area. It will also prevent some display issues in some browsers when pages contain Javascript pop-up boxes or drop-down menus and have the colors overridden.

**Procedure:**

1. Open the Web page in a browser that allows users to change colors of HTML content.
2. Change the text, link and background colors in the browser settings so they are different than those currently set in the browser.
3. Return to the page and check that it is sisplaying the page in the new text link and background colors.
4. Check that any borders are still displayed and that the layout is retained.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C25)

</details>

<details>
  <summary>What abjective of making the DOM order match the visual order?</summary>

The objective of this technique is to ensure that the order of content in the source code is the same as the visual presentation of the content. The order of content in the source code can be changed by the author to any number of visual presentations with CSS. Each order may be meaningful in itsef bu may cause confusion for assistive technology users.

**Procedure:**

1. Visually eamine the order of the content in the Web page as it is presented to the end user.
2. Examine the elements in the DOM using a tool that allows you to see the DOM.
3. Ensure that the order of the content in the source code sections match the visual presentation of the content in the Web page.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C27)

</details>
