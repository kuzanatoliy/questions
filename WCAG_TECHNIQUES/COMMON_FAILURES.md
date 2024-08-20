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

<details>
  <summary>What is a failure of success criterion 4.1.2 due to implementing custom controls that do not use an accessibility API for the technology, or do so incompletely?</summary>

When standard controls from accessible technologies are used, they usually are programmed in a way that uses and supports the accessibility API. However, when custom controls are created, it is up to the control's author to ensure that the control is correctly exposed to users via the platform's accessibility API. If this is not done, then assistive technologies will not be able to understand what the control is or how to operate it or may not even know of its existence.

**Procedure:**

1. Using the accessibility checker for the technology (or if that is not available, inspect the code using a browser's developer tools, or test with an assistive technology), check the controls to see if they support the accessibility API.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F15)

</details>

<details>
  <summary>What is a failure of success criterion 2.2.2 due to including scrolling content where movements is not essential to the activity without also including a mechanism to pause and restart the content?</summary>

In this failure technique, there is moving or scrolling content that cannot be paused and resumed by users. In this case, some users with low vision or congnitive disabilities will not be able to perceive the content.

**Procedure:**

1. Check that a mechanism is provided in the Web page or user agent to pause moving or scrolling content.
2. Use the puse mechanism to pause the moving or scrolling content.
3. Check that the moving or scrolling has stopped and does not restart by itself.
4. Check that a mechanism is provided in the Web page or user agent to restart the paused content.
5. Use the restart mechanism provided to restart the moving content.
6. Check that the movement or scrolling has resumed from the point where it was stopped.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F16)

</details>

<details>
  <summary>What is a failure of Conformance Requirement 1 due to not providing a method for the user to find the alternative conforming version of a non-conforming Web page?</summary>

This failure technique describes the situation in which an alternate, conforming version of the content is provided, but there is no direct way for a user to tell that it is available or where to find it. Such content fails the Success Criterion because the user cannot find the conforming version.

**Procedure:**

1. Identify a nonconforming page that has an alternative conforming version.
2. Determine if the nonconforming page provides a link to the conforming version.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F19)

</details>

<details>
  <summary>What is a failure of Success Criterion 1.1.1 and 4.1.2 due to not updating text alternatives when changes to non-text content occur?</summary>

This objective of this failure conditions is to address situations where the non-text content is updated, but the text alternative is not updated at the same time. If the text in the text alternative cannot still be used in place of the non-text content without losing information or function, then it fails because it is no longer a text alternative for the non-text content.

**Procedure:**

1. Check each text alternative to see if it is describing content other than the currently displayed non text content.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F20)

</details>

<details>
  <summary>What is a failure of Success Criterion 3.2.5 due to opening windows that are not requested by the user?</summary>

Failure due to opening new windows when the user does not expect them. New windows take the focus away from what the user is reading or doing. This is fine when the user has intacted with a piece of User Interface and expects to get a new window, such as an options dialogue. The failure comes when pop-ups appear unexpectedly.

**Procedure:**

1. Load the Web page.
2. Check if new (additional) windows open.
3. Find every actionalbe lement, such as links and buttons, in the Web page.
4. Activate each element.
5. Check if activation the element opens a new window.
6. Check if elements that open new windows have associated text saying that will happen. The text can be displayed in the link, or available through a hidden association such as an HTML title attribute.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F22)

</details>

<details>
  <summary>What is a failure of 1.4.2 due to playing a sound longer than 3 seconds where there is no mechanism to turn it off?</summary>

This describes a failure condition for Success Criteria involving sound. If sound does not turn off automatically within 3 seconds and there is no way to turn the sound off, independently from the overall system volume level, then Success Criterion 1.4.2 would not be met. The sound would fall within this failure condition.

**Procedure:**

1. Check tat there is a mechanism, independent from the overall system volume control, to turn off any sound that plays automatically for more than three seconds.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F23)

</details>

<details>
  <summary>What is a failure of Sucess Criterion 1.4.3, 1.4.6 and 1.4.8 due to specifying foreground colors without specifying backgfound colors or vice versa?</summary>

Users with vision loss or congnitive, language and learning challenges often prefer specific foreground and background color combinations. In some cases, individuals with low vision will find it much easier to see a Web page that has white text on a back background, and they may have set their user agent to present this contrast. Many user agent make it possible for users to choose apreference about the foreground or background colors they would like to see without overriding all author-specified styles. This makes it possible for users to view pages where colors have not been specified by the author in their preferred color combination.

**Procedure:**

1. Examine the code of the Web page.
2. Check to see if an author-specified foreground color is present.
3. Check to see if an author-specified background color is present.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F24)

</details>

<details>
  <summary>What is a failure of Sucess Criterion 2.4.2 due to the title of a Web page not identifying the contents?</summary>

This describes a failure condition when the Web page has a title, but the title does not identify the contents or purpose of the Web page.

**Procedure:**

1. Check whether the title of each Web page identifies the contents or purpose of the Web page.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F25)

</details>

<details>
  <summary>What is a failure of Sucess Criterion 1.3.3 due to using a graphical symbol alone to convey information?</summary>

The objective of this technique is to show how using a graphical symbol to convey information can make content difficult to comprehend. A graphical symbol may be an image, an image of text or a pictorial or decorative character symbol which imparts information nonverbally. Examples of graphical symbols include an image of a red circle with a line through it a 'smiley' face, or a glyph which represents a check mark, arrow, or other symbol but is not the character with that meaning.

**Procedure:**

1. Check whether there are other means to determine the information conveyed by the non-text marks.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F26)

</details>

<details>
  <summary>What is a failure of Sucess Criterion 1.1.1 and 1.2.1 due to using text alternatives that are not alternatives (e.g., filenames or placeholder text)?</summary>

This describes a failure condition for all techniques involving text alternatives. If the text in the "text alternative" connot be used in place of the non-text content without losing information or function then alternative to the non-text content.

**Procedure:**

1. Check each text alternative to see if it is not actually a text alternative for the non-text content.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F30)

</details>

<details>
  <summary>What is a failure of Sucess Criterion 3.2.4 due to using two different labels for the same function on different Web pages within a set of Web pages?</summary>

Components that have the same function in different Web pages are more easily recognized if they are labeled consistently. If the naming is not consistent, some users may get confused.

**Procedure:**

1. In a set of Web pages, find components with the same function that are repeated in miltiple Web pages.
2. For each component with the same function found in step #1, check that the naming is consistent.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F31)

</details>

<details>
  <summary>What is a failure of Sucess Criterion 1.3.2 due to using white space characters to control spacing within a word?</summary>

The objective of this technique is to describe how using white space characters, such as space, tab, line break, or carriage return, to format individual words visually can be a failure to present meaningful sequences properly. When blank caracters are inserted to control letter spacing within a word, they may change the interpretation of the word or cause it not to be programmatically recognized as a single word.

**Procedure:**

1. Check wheter any words in the text of the content contain white space characters.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F32)

</details>

<details>
  <summary>What is a failure of Sucess Criterion 1.3.1 and 1.3.2 due to using white space characters to create multiple columns in plain text content?</summary>

The objective of this technique is to describe how using white space characters, such as space, tab, line break, or carriage return, to format columns of data in text content is a failure to use structure properly. Assistive technologies will interpret content in the reading order of the current language. Using white space characters to create multiple columns does not provide the information in a natural reading order. Thus, the assistive technology user will not be presented with the information in an understandable manner.

**Procedure:**

1. Examine the document for data or information presented in columnar format.
2. Check whether the columns are created using white space characters to lay out the information.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F33)

</details>

<details>
  <summary>What is a failure of Sucess Criterion 1.3.1 and 1.3.2 due to using white space characters to format tables in plain text content?</summary>

The objective of this technique is to describe how using white space characters, such as space, tab, line break, or carriage return, to format tables in text content is a failure to use structure properly. When tables are created in this manner there is no way to indicate that a cell is intended to be a header cell, no way to associate the table header cells with the table data cells, or to navigate directly to a particular cell in a table.

**Procedure:**

1. Examine the document for visually formatted tables.
2. Check whether the tables are created using white space characters to layout the tabular data.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F34)

</details>

<details>
  <summary>What is a failure of Sucess Criterion 3.2.2 due to automatically submitting a form and presenting new content without prior warning when the last field in the form is given a value?</summary>

Forms are frequently designed so that they submit automatically when the user has filled in all the fields, or when focus leaves the last field. There are two problems with this approach. First is that a disabled user who needs more context may move focus away from the field to the directions on how to fill in the form, or to other text, accidentally submitting the form. The other is that, with some form elements, the value of the field changes as each item is navigated with the keyboard again accidentally submitting the form. It is better to rely on the standard form behavior of the submit button and enter key.

**Procedure:**

1. Enter data in all fields on page starting at top.
2. Enter data in last fields and exit from it (tab out of it).
3. Check whether leaving the last field causes change of context.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F36)

</details>

<details>
  <summary>What is a failure of Sucess Criterion 3.2.2 due to launching a new window without prior warning when the selection of a radio button, check box or select list is changed?</summary>

This document describes a failure that occurs when changing the selection of a radio button, a check box or an item in a select list causes a new window to open. It is possible to use scription to create an input element that causes a change of context when the element is selected. Developers can instead use a sumbit button or clearly indicate the expected action.

**Procedure:**

1. Find each form in a page.
2. For each form control that is a radio button, check box or an item in a select list, check if changing the selection of the control launches a new window.
3. For each new window resulting from step 2, check if the user is warned in advance.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F37)

</details>

<details>
  <summary>What is a failure of Sucess Criterion 1.1.1 due to not marking up decorative images in HTML in a way that allows assistive technology to ignore them?</summary>

This describes a failure condition for text alternatives for images that should be ignored by AT. If there is no alte attribute at all assistive technologies are not able to ignore the non-text content. The alt attribute must be provided and have a null value to avoid a failure of this Success criterion.

**Procedure:**

1. Check whether the element has no role attribute or has a role attribute value that is not presentation.
2. Check whether the lement has no alt attribute or has an alt attribute with a value that is not null.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F38)

</details>

<details>
  <summary>What is a failure of Sucess Criterion 1.1.1 due to provideing text alternative that is not null for images that should be ignored by assistive technology?</summary>

This texhnique describes a failure condition for images that should be ignored by assistive technologies. A text alternative for an image should convey the meaning of the image. When an image is used for decoration, spacing or other purpose that is not part of the meaningful content in the page then the image has no meaning and should be ignored by assistive technologies.

**Procedure:**

1. Identify and img elements that are used for decoration, spacing or other purpose that is not part of the meaningful content in the page.
2. Check that the alt attribute for these elements is null.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F39)

</details>

<details>
  <summary>What is a failure due to using meta redirect with a time limit?</summary>

Meta http-equiv content="{time} url=..." is often used to automatically redirect users. When occurs after a time delay, it is an unexpected change of context that may interrupt the user.

**Procedure:**

1. Check that the numerical value for seconds until refresh in the content attribute is present.
2. Check that the numerical value for seconds until refresh in the content attribute is less than one or greater than 72,000.
3. Check if the page qualifies for Real-time or Essential Exceptions in Success Criterion 2.2.1 Timing Adjustable.
4. Check if the user is provided an opportunity to turn off, extend, or adjust the timing of the page refresh.
5. Check if the page does not redirect after the duration specified in the content attribute.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F40)

</details>

<details>
  <summary>What is a failure of Success Criterion 2.2.1, 2.2.4, and 3.2.5 due to using meta refresh to reload the page?</summary>

Meta http-equiv of refresh is often used to periodically refresh pages or to redirect users to another page. If the time interval is too short, and there is no way to turn auto-refresh off, people who are blind will not have enough time to make their screen readers read the page before the page refreshes unexpectedly and causes the screen reader to begin reading at the top. Sighted users may also be disoriented by the unexpected refresh.

**Procedure:**

1. Check that the numerical value for seconds until refresh in the content attribute is present.
2. Check that the numerical value for seconds until refresh in the content attribute is less than one or greater than 72,000.
3. Check if the page qualifies for Real-time or Essential Exceptions in Success Criterion 2.2.1 Timing Adjustable.
4. Check if the user is provided an opportunity to turn off, extend, or adjust the timing of the page refresh.
5. Check if the page does not redirect after the duration specified in the content attribute.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F41)

</details>

<details>
  <summary>What is a failure of Success Criterion 1.3.1, 2.1.1, 2.1.3 or 4.1.2 when emulating links?</summary>

This failure occurs when JavaScript event handlers are attached to elements to emulate links. A link created in this manner cannot be tabbed to from the keyboard and does not gain keyboard focus like other controls and/or links. If scripting events are used to emulate links, user agents including assistive technology may not be able to identify the links in the content as links. They may be recognized as interactive controls but still not recognized as links. Such elements do not appear in the links list generated by user agents or assistive technology.

**Procedure:**

1. Check if the programmatically determined role of the element is "link".
2. Check if the emulated link can be activated using the keyboard.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F42)

</details>

<details>
  <summary>What is a failure of Success Criterion 1.3.1 due to using structural markup in a way that does not represent relationships in the content?</summary>

This objective of this technique is to describe a failure that occurs when structural markup is used to achive a presentational effect, but indicates relationships that do not exist in the content. This is disorienting to users who are depending on those relationships to navigate the content or to understand the relationship of one piece of the content to another. Note that the structural markup such as `<th>` or `<caption>` elements.

**Procedure:**

1. Check that the element's semantic meaning is exposed to assistive technology and appropriate for the content of the element.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F43)

</details>

<details>
  <summary>What is a failure of Success Criterion 2.4.3 due to using tabindex to create a tab order that does not preserve meaning and operability?</summary>

One of the most common causes of this failure occurs when editing a page where tabindex has been used. It is easy for the tab order and the content order to fall out of correspondence when the content is edited but the tabindex attributes are not updated to reflect the changes to the content.

**Procedure:**

1. If tabindex is used, check that the tab order specified by the tabindex attributes follows relationships in the content.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F44)

</details>

<details>
  <summary>What is a failure of Success Criterion 1.3.1 due to using th elements, caption elements, or non-empty summary attributes in layout tables?</summary>

The objective of this technique is to describe a failure that occurs when a table used only for layout includes either th elements, a summary attribute, or a caption element. This is a failure because it uses structural (or semantic) markup only for presentation. The intent of the HTML table elements is to present data.

**Procedure:**

1. Examine the source code of the HTML or XHTML document for the table element.
2. If the table is used only to visually lay out elements within the content.

- Check that the table does not contain any th elements.
- Check that the table element does not contain a non-empty summary attribute.
- Check tat the table element does not contain a caption element.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F46)

</details>

<details>
  <summary>What is a failure of Success Criterion 2.2.2 due to using the blink element?</summary>

The blink element, while not part of the official HTML specification, is supported by many user agents. It causes any text inside the element to blink at a predetermined rate. This cannot be interrupted by the user, nor can it be disabled as a preference. The blinking continues as long as the page is displayed. Therefore, content that uses blink fails the Success Criterion because blinking can continue for more than three seconds.

**Procedure:**

1. Examine code for the presence of the blink element.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F47)

</details>

<details>
  <summary>What is a failure of Success Criterion 1.3.1 due to using the pre element to markup tabular information?</summary>

This document describes a failure caused by use of the HTML pre element to markup tabular information. The pre element preserves only visual formatting. If the pre element is used to markup tabular information, the visually inmpied logical relationships between the table cells and the headers are lost if the user cannot see the screen or if the visual presentation changes significantly.

**Procedure:**

1. Check to see if the pre element is used.
2. For each occurrence of the pre element, check whether the enclosed information is tabular.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F48)

</details>

<details>
  <summary>What is a failure of Success Criterion 1.3.2 due to using an HTML layout table that does not make sense when linearized?</summary>

This failure occurs when a meaningful sequence of content conveyed through presentation is lost because HTML tables used to control the visual placement of the content do not 'linerize' correctly. Tables present content in two visual dimensions, horizontal and vertical. However, screen readers present this two-dimensional content in linear order of the content in the source, beginning with the first cell in the first row and ending with the last cell in the last row. The screen reader reads the table from top to bottom, reading the entire contents of each row before moving to the next row. The completer content of each cell in each row is spoken - including the complete content of any table nested within a cell. This is called linearization.

**Procedure:**

1. Linearize the content in either of the following ways:

- Present the content in source code order;
- Remove the table markup from around the content.

2. Check that the linear reading order matches any meaningful sequence conveyed through presentation.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F49)

</details>

<details>
  <summary>What is a failure of Success Criterion 2.2.2 due to a script that causes a blink effect without a mechanism to stop the blinking at 5 seconds or less?</summary>

Scripts can be used to blink content by toggling at 5 seconds or earlier. See using scripts to control blinking and stop it in five seconds or less for information about how to modify the technique to stop the blinking.

**Procedure:**

1. Determine if the blinking stops in 5 seconds or less.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F50)

</details>

<details>
  <summary>What is a failure of Success Criterion 3.2.1 and 3.2.5 due to opening a new window as soon as a new page is loaded?</summary>

Some Web sites open a new window when a page is loaded, to advertise a product or service. The objective of this technique is to ensure that pages do not disorient users by opening up one or more new windows that automatically attain focus as soon as a page is loaded.

**Procedure:**

1. Load a new page.
2. Check to see whether a new window has been opened as a result of loading the new page.
3. Check to see whether the new window is automatically given focus.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/failures/F52)

</details>