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

<details>
  <summary>What abjective of specifying the size of text containers using em units?</summary>

The objective of this technique is to specify the width and/or height of containers, that contain thext or that will accept text input, in em units. This will allow user agents that support text resizing to resize the text containers in line with changes in text size settings.

**Procedure:**

1. Identify containers that contain text or allow text input.
2. Check the container's width and/or height are specified in em units.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C28)

</details>

<details>
  <summary>What abjective of using a style switcher to provide a conforming alternate version?</summary>

The objective of this technique is to demonstrate how CSS can be used in combination with scripting to provide conforming alternate versions of a Web page. In this technique, an author provides alternative views of the content by providing controls that adjust the CSS that is used to control the visual presentation of content. Controls provided withing the Web page allow users to select or modify the presentation in a way that meets the success criterion at the level claimed.

**Procedure:**

1. Check that the Web page contains controls that allow users to select alternate presentations.
2. Check that the control changes the presentation by modifying individual CSS style properties or by activationg an alternate style sheet.
3. Verify that the resulting page is a conforming alternate version for the original page.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C29)

</details>

<details>
  <summary>What abjective of using CSS to replace text with images of text and providing user interface controls to switch?</summary>

The objective of this technique is to demonstrate how CSS can be used to replace structured HTML text with images of text in a way that makes it possible for users to view content according to their preferences. To use this technique, an author starts by creating an HTML page that uses semantic elements to mark up the structure of the page. The autor then designs two or more stylesheets for that page. One stylesheet presents the HTML text as text and the second uses CSS features to replace some of the HTML text with images of text. Finally, though the use of server-size or client-side scripting, the author provides a control that allows the user to switch between the available views.

**Procedure:**

1. Check that the Web page includes a control that allows users to select an alternate presentation.
2. Check that when the control is activated the resulting page includes text (programmatically determined text) wherever images of text had been used.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C30)

</details>

<details>
  <summary>What abjective of using CSS Flexbox to reflow content?</summary>

The objective of this technique is to present content without introducing a horizontal scroll bar at a width equivalent to 320 CSS pixels, or a vertical scroll bar at a height equivalent to 256 CSS pixels for text intended to scroll horizontally. This is done by using layout techniques that adapt to the available viewport space.

**Procedure:**

1. Display the web page in a user agent capable of 400% zoom and set the viewport dimensions (in CSS pixels) to 1280 wide and 1024 high.
2. Zoom in by 400%.
3. For content read horizontally, check that all content and functionality is available without horizontal scrolling.
4. For content read vertically, check tat all content and functionality is available without vertical scrolling.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C31)

</details>

<details>
  <summary>What abjective of using media queries and grid CSS to reflow columns?</summary>

The objective of this technique is to be able to present content without introducing a horizontal scroll bar at a width equivalent to 320 CSS pixels, or a vertical scroll bar at a height equivalent to 256 CSS pixels for text intended to scroll horizontally. This is done using layout techniques that adapt to the available viewport space.

**Procedure:**

1. Display the web page in a user agent capable of 400% zoom and set the viewport dimensions (in CSS pixels) to 1280 wide and 1024 high.
2. Zoom in by 400%.
3. For content read horizontally, check that all content and functionality is available without horizontal scrolling.
4. For content read vertically, check tat all content and functionality is available without vertical scrolling.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C32)

</details>

<details>
  <summary>What abjective of allowing for reflow with Long URLs and Strings of Text?</summary>

Long sets of characters without a space, such as URLs shown as content, can break reflow when the page is zoomed. The objective of this technique is to present URLs without introducing a horizontal scroll bar at a width equivalent to 320 CSS pixels or a vertical scroll bar at a height equivalent to 256 CSS pixels. This is done by using CSS techniques that adapt to the available viewport space. Note: Using a human readable text link, rather than a long URL, is better for usability and accessibility.

**Procedure:**

1. Display the web page in a user agent capable of 400% zoom and set the viewport dimensions (in CSS pixels) to 1280 wide and 1024 high.
2. Zoom in by 400%.
3. For content read horizontally, check that all content and functionality is available without horizontal scrolling.
4. For content read vertically, check tat all content and functionality is available without vertical scrolling.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C33)

</details>

<details>
  <summary>What abjective of using media queries to un-fixing sticky headers / footers?</summary>

The objective of this technique is to be able to present content with sticky headers and footers when there is enough space. This is done by using min-height, max-height, and min-width media queries techniques that adapt to the available space of the viewport.

**Procedure:**

1. Display content of a device / user agent in portrait mode.
2. Change the orientation to landscape.
3. Check whether the sticky header and footer will be un-fixed depending on the existing media query settings.
4. Display content on a desktop / user agent at a starting viewport width of 1280x1024 CSS pixels.
5. Change the viewport size in width and height or use the zoom function of the browser.
6. Check whether the sticky header and footer will be un-fixed at specific sizes depending on the existing media query settings.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C34)

</details>

<details>
  <summary>What abjective of allowing for text spacing without wrapping?</summary>

The objective of this technique is to allow a user to override text spacgin via user stylesheet, bookmarklet, extension, or application. Increased spacing between paragraphs, lines, words, and characters benefits people with low vision or some cognitive disabilities. Content needs to allow spacing changes without loss of content or functionality by allowing the elements containing the text to expand as needed.

**Procedure:**

1. Set zoom level to 100%.
2. Use a tool or another mechanism to apply the text spacing metrics (line height, and paragraph, letter, and word spacing), such as the Text Spacing Bookmarklet or a user style browser plugin.
3. Check that all content and functionality is available e.g., text in containers is not truncated and does not overlap other content.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C35)

</details>

<details>
  <summary>What abjective of allowing for text spacing override?</summary>

The objective of this technique is to allow a user to override text spacgin via user stylesheet, bookmarklet, extension, or application. Increased spacing between paragraphs, lines, words, and characters benefits people with low vision or some cognitive disabilities. Content needs to allow spacing changes without loss of content or functionality, so text containers must either have room for the text to expand or the container must be able to expand. This technique will typically apply to short strings of text such as in a navigation bar, as longer strings of text are increasingly likely to require wrapping to be readable when styles are changed.

**Procedure:**

1. Set zoom level to 100%.
2. Use a tool or another mechanism to apply the text spacing metrics (line height, and paragraph, letter, and word spacing), such as the Text Spacing Bookmarklet or a user style browser plugin.
3. Check that all content and functionality is available e.g., text in containers is not truncated and does not overlap other content.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C36)

</details>

<details>
  <summary>What abjective of using CSS max-width and height to fit images?</summary>

The objective of this technique is to be able to present images without introducing a horizontal scroll bar at a width equivalent to 320 CSS pixels, or a vertical scroll bar at a height equivalent to 256 CSS pixels for content intended to scroll horizontally. This is done by using CSS max-width and height property techniques that adapt to the available space and keep the original demensions of the image.

**Procedure:**

1. Display the web page in a user agent capable of 400% zoom and set the viewport dimensions (in CSS pixels) to 1280 wide and 1024 high.
2. Zoom in by 400%.
3. For content read horizontally, check that all images fit in their available space without horizontal scrolling.
4. For content read vertically, check that all images fit in their available space without vertical scrolling.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C37)

</details>

<details>
  <summary>What abjective of using CSS width, max-width and flexbox to fit labels and inputs?</summary>

The objective of this technique is to be able to present labels and inputs without introducing a horizontal scroll bar at a width equivalent to 320 CAA pixels for content intended to scroll vertically. When space is limited in the viewport for the label and input to sit next to each other horizontally, they will be changed to a vertical alignment. This is done by using CSS properties for width, max width and flexbox that adapt to the availble space.

**Procedure:**

1. Display the web page in a user agent capable of 400% zoom and set the viewport dimensions (in CSS pixels) to 1280 wide and 1024 high.
2. Zoom in by 400%.
3. For vertically scrolling content, all labels and inputs fit in their available space without horizontal scrolling.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C38)

</details>

<details>
  <summary>What abjective of using the CSS reduce-motion query to prevent motion?</summary>

The objective of this technique is to allow users to prevent animation from being displayed on Web pages, via the use of the prefers-reduced-motion CSS Media Query.

**Procedure:**

1. Enable the 'Reduce Motion' setting in your system;
2. Check that the motion is not essential;
3. Check taht the element does not move.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C39)

</details>

<details>
  <summary>What abjective of creating a two-color focus indicator to ensure sufficient contrat with all components?</summary>

The objective of this technique is to create a two-color focus indicator that has sufficient contrast against any solid background color. This technique can avoid the need for multiple classes to ensure sufficient contrast of the focus indicator when viewed against different backgrounds.

**Procedure:**

1. Check that the two colors in the focus indicator have a contrast ratio that is 9:1 or greater with each other.
2. Check that each color band is at least 2 CSS pixels thick.
3. Check that the indicator only appears overtop one solid background color at a time.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C40)

</details>

<details>
  <summary>What abjective of creating a strong focus indicator within the component?</summary>

The objective of this technique is to create a highly visible focus indicator that has sufficient contrast against the internal background color of a component.

**Procedure:**

1. Place keyboard focus on each focusable user interface element on the page using the keyboard.
2. Check that the focus indicator area is at least the size of a 2 CSS px border around the component.
3. Check that the change of contrast of the indicator between focused andd unfocused states has a ratio of 4.5:1 for the minimum focus indicator area.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C41)

</details>

<details>
  <summary>What abjective of using min-height and min width to ensure sufficient target spacing?</summary>

The objective of this technique is to ensure that links in navigation or pagination menus will be spaced so that they fall within an area that measures at least 44 x 44 CSS pixels if the target area itself is smaller than that. The aim is to provide an adequate target clearance so the offset to adjacent targets is sufficent to prevent accidental pointer activation of adjacent targets.

**Procedure:**

1. Check tat the target has enough spacing so that the space around it measures at least 44px width and 44px height.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/C42)

</details>
