# Common failures

<details>
  <summary>What is a failure of success criterion 1.3.2 due to changing the meaning of content by positioning information with CSS?</summary>

The describes the failure condition that results when CSS, rather than structural markup, is used to modify the visual layout of the content, and the modified layout changes the meaning of the content. Using the positioningproperties of CSS2, content may be displayed at any position on the user's viewport. The order in which items appear on a screen may be different than the order they are found in the source document. Assistive technologies rely on the source code or other programmatically determined order to render the content in the correct sequence. Thus, it is important not to rely on CSS to programmatically determined reading order.

**Procedure:**

1. Remove the style infromation from the document or turn off use of style sheets in the user agent.
2. Check that the reading order of the contnent is correct and the meaning of the content is preserved.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F1)

</details>

<details>
  <summary>What is a failure of success criterion 1.3.1 due to using changes in text presentation to convey information without using the appropriate markup or text?</summary>

The failure occurs when a change in the appearance of text conveys meaning without using appropriate semantic markup. This failure also applies to images of text that are not enclosed in the appropriate semantic markup.

**Procedure:**

1. For images of text:

- Check if any images of text are used to convey structural information of the document.
- Check that the proper semantic structure (e.g., HTML headings) is used with the text to convey the information.

2. For styled text that conveys information:

- Check if there is any styled text that conveys structural information.
- Check that in addition to styling, the proper semantic structure is used with the text to convey the information.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F2)

</details>

<details>
  <summary>What is a failure of success criterion 1.1.1 due to using CSS to include images that convey important information?</summary>

The CSS background image property provides a way to include images in the document with CSS without any reference in the HTML code. The CSS background-image property was designed for decorative purposes and it is not possible to associate text alternative with images that are included via CSS. Text alternatives are necessary for people who cannot see images that convey important information. Therefore, it is a failure to use this property to add images to convey important information. This failure would apply equally in a case where the background image was declared in the HTML style attribute, as well as in a case where the background image declaration was created dynamically in a client script.

**Procedure:**

1. Examine all images added to the content via CSS, HTML style attributes, or dynamically in script as background images.
2. Check that the images do not convey important information.
3. If an image does convey important information, the information is provided to assistive technologies and is also available when the CSS image is not displayed.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F3)

</details>
