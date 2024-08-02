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

<details>
  <summary>What is a failure of success criterion 2.2.2 due to using text-decoration:blink without a mechanism to stop it in less than five seconds?</summary>

CSS defines the blink value for the text-decoration property. When used, it causes any text in elements with this property to blink at a predetermined rate. This cannot be interrupted by the user, nor can it be disabled as a user agent preference. The blinking continues as long as the page is displayed. Therefore, content that uses text-decoration:blink fails the Success Criterion because blinking can continue for more than five seconds.

**Procedure:**

1. Examine inline styles, internal stylesheets, and external stylesheets for the text-decoration property with a value of blink.
2. If the property is used, determine if the ID class, or element identified by selectors on which this property is defined are used in the document.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F4)

</details>

<details>
  <summary>What is a failure of success criterion 2.2.2 due to an object or appliet that has blinking content without a mechanism to pause the content that blinks for more than five seconds?</summary>

When content that is rendered by a plug-in or contained in an applet blinks, there may be no way for the user agent to pause the blinking. If neither the plug-in, applet, nor the content itself provides a mechanism to pause the content the user may not have sufficient time to read the content between blinks or it may be so distracting that the user will not be able to read other content on the page.

**Procedure:**

1. Determine if the content continues to blink for longer than 5 seconds.
2. Determine if there is a means to pause the blinking content.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F7)

</details>

<details>
  <summary>What is a failure of success criterion 1.2.2 due to captions omitting some dialogue or important sound effects?</summary>

This describes a failure condition for all techniques involving captions. If the "caption" does not include all of the dialogue (eigher verbatim or in essence) as well as all important sounds then the 'Captions' are not real captions.

**Procedure:**

1. View the material with captioning turned on.
2. Check that all dialogue is accompanied by a caption.
3. Check that all important sounds are captioned.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F8)

</details>
