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

<details>
  <summary>What is a failure of success criterion 2.1.2 and conformance requirement 5 due to combining multiple content formats in a way that traps users inside one format type?</summary>

When content includes miltiple formats, one or more user agent or plug-ins are often needed in order to successfully present the content to users. For example, a page that includes HTML, SVG, SMIL and XFroms may require a browser to load as many as three different plug-ins in order for a user to successfully interact with the content. Some plug-ins create a common situation in which the keyboard focus can become "stuck" in a plug-in, leaving a keyboard-only user with no way to return to the other content.

**Procedure:**

1. Using a keyboard, navigate through the content.
2. Check to see that the keyboard focus is not "trapped" and it is possible to move keyboard focus out of the plug-in content without closing the user agent or restarting the system.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F10)

</details>

<details>
  <summary>What is a failure of success criterion 2.2.5 due to having a session time limit without a mechanism for saving user's time limit without a mechanism for saving user's input and re-establishing that information upon re authentication?</summary>

Web servers that require user authentication usually have a session mechanism in which a session times out after a period of inactivity from the user. This is sometimes done for security reasons, to protect users who are assumed to have left their computer expsed in a state where someone could do something harmful to them such as transfer bank funds or make an unauthorized purchase. Users with disabilities may actually still be working to complete the form as it may take them longer to complete the form than would normally be expected Upon re-authentication, if the state of users' sessions are not restored, including all data that had been previously entered into the form, they will have to start over. And for these users, it is likely that the session will time out again before they can complete the form. This sets up a situation where a user who needs more time to complete the form can never complete it.

**Procedure:**

1. Provide user input as required but allow the session to time out, then submit the form.
2. When requested, re-authenticate with the server.
3. Determine if the function is performed using the previously submitted data.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F12)

</details>

<details>
  <summary>What is a failure of success criterion 1.1.1 and 1.4.1 due to having a text alternative that does not include information that is conveyed by color differences in the image?</summary>

The objective of this technique is to describe the failure that occurs when an image uses color differences to convey information, but the text alternative for the image does not convey that information. This can cause problems for people who are blind or colorblind because they will not be able to perceive the information conveyed by the color differences.

**Procedure:**

1. Check that the information conveyed by color differences is not included in the text alternative for the image.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F13)

</details>

<details>
  <summary>What is a failure of success criterion 1.3.3 due to identifying content only by its shape or location?</summary>

The objective of this technique is to show how indentifying content only by its visual shape or location makes content difficult to understand and operate. When only visual identification or location is used, users with visual disabilities may find it difficult to locate content since they cannot see the screen or may perceive only a small portion of the screen at one time. Also, location of content can vary if page layout varies due to variations in font, window, or screen size.

**Procedure:**

1. Examine the Web page for textual references to content within the Web page.
2. Check that the references do not rely on only the visual shape or location of the content.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F14)

</details>
