# Client-Side Script Techniques

<details>
  <summary>What abjective of allowing the user to extend the default time limit?</summary>

The objective of this technique is to allow user to extend the default time limit by providing a mechanism to extend the time when scripts provide functionality that has default time limits. In order to allow the user to request a longer time limit, the script can provide a form allowing the user to enter a larger time limit or indicating that more time is needed.

**Procedure:**

1. On a Web page that uses scripts to enforce a time limit, wait until the time limit has expired.
2. Determine if an option was provided to extend the time limit.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR1)

</details>

<details>
  <summary>What abjective of using redundant keyboard and mouse event handlers?</summary>

The objective of this technique is to demonstrate using device independent events to change a decorative image in response to a mouse or focus event. Use the onmounseover and onmouseout events to change a decorative image when the mouse moves on top of or away from an element on the page. Also, use the onfocus and onblur events to change the image when the element receives and loses focus.

**Procedure:**

1. Check that the "standard" image is displayed as expected when the Web page is loaded.
2. Using the mouse:

- Move the mouse over the element containing the event handlers (in this example it is an anchor element). Check that the image changes to the expected image.
- Move the mouse off of the element. Check that the image changes back to the "standard" image.

3. Using the keyboard:

- Use the keyboard to set focus to the element containing the event handlers. Check that the image changes to the expected image.
- Use teh keyboard to remove focus from the element (generally by moving focus to another element). Check that the image changes to the "standard" image.

4. Verify that the layout of other elements on the page is not affected when the image is changed.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR2)

</details>

<details>
  <summary>What abjective of using scripts to make nonessential alerts optional?</summary>

The objective of this technique is to toggle announcements to screen readers of changes in a stock-price alert component. By default, when the stock price changes, the change is announced by screen readers. Thsi could be annoying to some users, so there are buttons to allow users to toggle the announcements on or off.

**Procedure:**

1. Load the Web page and verify that no non-emergency alerts are displayed.
2. Verify there is a mechanism to activate and deactiveate the non-emergency interruptions.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR14)

</details>

<details>
  <summary>What abjective of providing a script that warns the user a time limit is about to expire?</summary>

The objective of this technique is to notify users that they are almost out of time to complete an interaction. When scripts provide functionality that has time limits, the script can include functionality to warn the user of imminent time limits and provide a mechanism to request more time.

**Procedure:**

1. Load the page and start a timer that is 20 seconds less than the time limit.
2. When the timer expires, check that a confirmation dialog is displayed warning of the impending time limit.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR16)

</details>

<details>
  <summary>What abjective of providing client-side validation and alert?</summary>

The objective of this technique is to validate user input as values are entered for each field, by means of client-side scripting. If errors are found, an alert dialog describes the nature of the error in text. Once the user dismisses the alert dialog, it is helpful if the script positions the keyboard focus on the field where the error occurred.

**Procedure:**

1. Enter invalid data.
2. Determine if an alert describing the error is provided.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR18)

</details>

<details>
  <summary>What abjective of using an onchange event on a select element without causing a change of context?</summary>

The objective of this technique is to demonstrate how to correctly use an onchange event with a select element to update other elements on the Web page. This technique will not cause a change of context. When there are one or more select elements on the Web page, an onchange event on one, can update the options in another select element on the Web page. All of the data required by the select elements is included within the Web page.

**Procedure:**

1. Navigate to the trigger select element (in this example, the one to select continents) and change the value of the select.
2. Navigate to the select element that is updated by the trigger (in this example, the one to select conuntries).
3. Check that the matching option values are displayed in the other select element.
4. Navigate to the trigger select element, navigate through the options but do not change the value.
5. Check that the matching option values are still displayed in the associated element.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR19)

</details>

<details>
  <summary>What abjective of using both keyboard and other device specific functions?</summary>

The objective of this technique is to illustrate the use of both keyboard-specific and mouse specific events with code that has a scription fuction associated with an event. Using both keyboard-specific and mouse specific events together ensures that content can be operated by a wide range of devices. For example, a script may perform the same action when a keypress is detected that is performed when a mouse button is clicked. This technique goes beyond the Success Criterion requirement for keyboard access by including not only keyboard access but access using other devices as well.

**Procedure:**

1. Find all interactive functionality.
2. Check that all interactive functionality can be accessed using the keyboard alone.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR20)

</details>

<details>
  <summary>What abjective of using scripts to control blinking and stop it in five seconds or less?</summary>

The objective of this technique is to control blinking with script so it can be set to stop in less than five seconds by the script. Script is used to start the blinking effect of content, control the toggle between visible and hidden states, and also stop the effect at five seconds or less. The setTimeout() function can be used to toggle blinking content between visible and hidden states, and stop when the number of interations by the time between item adds up to nearly five seconds.

**Procedure:**

1. Start a timer for 5 seconds at the start of the blink effect.
2. When the timer expires, determine if the blinking has stopped.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR22)

</details>

<details>
  <summary>What abjective of using progressive enhancement to open new windows on user request?</summary>

The objective of this technique is to avoid confusion that may be caused by the appearance of new windows that were not requested by the user. Suddenly opening new windows can disorient or be missed completely by some users. New windows / tabs can be opened with the HTML target attribute or JavaScript. The example below demonstrates how to open new windows with script: it adds an event handler to a link and warns the user that the content will open in a new window.

**Procedure:**

1. Activate each link in the document to check if it opens a new window.
2. For each link that opens a new window, check tat it uses script to accomplish each of the following:

- indicates that the link will open in a new window,
- uses device independent event handlers, and
- allows the browser to open the content in the same window if a new window was not opened.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR24)

</details>

<details>
  <summary>What abjective of inserting dynamic content into the Document Object Model immediately following its trigger element?</summary>

The objective of this technique is to place inserted user interface elements into the Document Object Model (DOM) in such a way that the tab order and screen-reader reading order are set correctly by the default behavior of the user agent. This technique can be used for any user interface element that is hidden and shown, such as menus and dialogs.

**Procedure:**

1. Find all areas of the page that trigger dialogs that are not pop-up windows.
2. Check that the dialogs are triggered from the click event of a button or a link.
3. Using a toll that allows you to inspect the DOM generated by script, check that the dialog is next in the DOM.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR26)

</details>

<details>
  <summary>What abjective of reordering page sections using the Document Object Model?</summary>

The objective of this technique is to provide a mechanism for re-ordering component which is both highly usable and accessible. The two most common mechanisms for reordering are to send users to a set-up page where they can number components, or to allow them to drag and drop components to the desired location.

**Procedure:**

1. Find all components in the Web Unit which can be reordered via drag and drop.
2. Check that there is also a mechanism to reorder them using menus build of lists of links.
3. Check that the menus are contained within the re-orderable items in the DOM.
4. Check that scripts for reordering are triggered only from the onclick event of links.
5. Check that items are reordered in the DOM, not only visually.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR27)

</details>

<details>
  <summary>What abjective of using an expandable and collapsible menu to bypass block of content?</summary>

This technique allows users to skip repeated material by placing that material in a menu that can be expanded or collpsed under user control. The user can skip the repeated material by collapsing the menu. The user invokes a user interface control to hide or remove the elements of the menu. The resources section lists several techniques for menus, toolbars and trees, any of which can be used to provide a mechanism for skipping navigation.

**Procedure:**

1. Check that some user interface control allows the repeated content to be expanded or collapsed.
2. Check that when the content is expanded, it is included in the programmatically determined content at a logical place in the reading order.
3. Check that when the content is collapsed, it is not part or the programmatically determined content.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR28)

</details>

<details>
  <summary>What abjective of adding keyboard-accessble actions to static HTML elements?</summary>

The objective of this technique is to demonstrate how to provide keyboard access to a user interface control that is implemented by actions to static HTML elements such as div or span. This technique ensures that the element is focusable by setting the tabindex attribute, and it ensures that the action can be triggered from the keyboard by providing an onkeyup or onkeypress handler in addition to an onclick handler.

**Procedure:**

1. Click on the control with the mouse.
2. Check that the scription action executes properly.
3. Check that it is possible to naigate to and give focus to the control via the keyboard.
4. Set keyboard focus to the control.
5. Check that pressing Enter or Space invokes the scription action.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR29)

</details>

<details>
  <summary>What abjective of using scripts to change the link text?</summary>

The purpose of this technique is to allow users to chooose to have additional information added to the text of links so that the links can be understood out of context.

**Procedure:**

1. Check that there is a link near the beginning of the page to expand links.
2. Check that the link identified in step 1 can be identified from link text alone.
3. Find any links on the page that cannot be identified from link text alone.
4. Activate the control identified in step 1.
5. Check taht the purpose of the links identified in step 3 can now be identified from link text alone.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR30)

</details>

<details>
  <summary>What abjective of providing client-side validation and adding error text via the DOM?</summary>

The objective of this technique is to demonstrate the display of an error message when client side validation of a form field has failed. Anchor elements are used to display the error messages in a list and are inserted above the fields to be validated. Anchor elements are used in the error messages so that focus can be placed on the error messages(s), drawing the user's attention to it. The href of the anchor elements contain an in-page link which references the fields where error(s) have been found.

**Procedure:**

1. Load the page.
2. Enter a valid value in the field(s) associated with an error message and verify that no error messages are displayed.
3. Enter an invalid value in the field(s) associated with an error message and verify that the correct error message for the field is displayed.
4. Verify that the error messages receive focus.
5. Enter a valid value in the field(s) associated with the displayed error message and verify that the error message is removed.
6. Repeat for all fileds with associated error messages created viea anchor tags.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR32)

</details>

<details>
  <summary>What abjective of using script to scroll content, and providing a mechanism to puase it?</summary>

The objective of this technique is to provide a way for users to stop scrolling content when the scrolling is created by a script. Scrolling content can be diffficult or impossible to read by users with low vision or with congnitive disabilities. The movement can also be distracting for some people making it difficult for them to concentrate on other parts of the Web page.

**Procedure:**

1. Check that a mechanism is provided to puase the scrolling content.
2. Use the pause mechanism to pause the scrolling content.
3. Check that the scrolling has stopped and does not restart by itself.
4. Check that a mechanism provided to restart the scrolling content.
5. Use the restart mechanism provided to restart the scrolling content.
6. Check that the scrolling has resumed from the point where it was stopped.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR33)

</details>

<details>
  <summary>What abjective of calculating size and position in a way that scales with text size?</summary>

The objective of this technique is to calculate the size and position of elements in a way that will scale appropriately as the text size is scaled.

**Procedure:**

1. Open a page that is designed to adjust container sizes as text size changes.
2. Increase the text size up to 200% using the browser's text size adjustment (not the zoom feature).
3. Examine the text to ensure the text container size is adjusted to accommodate the size of the text.
4. Ensure that no text is "clipped" or has disappeared as a result of the increase in text size.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR34)

</details>

<details>
  <summary>What abjective of making actions keyboard accessible by using the onclick event of anchors and buttons?</summary>

The objective of this technique is to demonstrate how to invoke a scripting function in a way that is keyboard accessible by attaching it to a keyboard-accessible control.

**Procedure:**

1. In a user agent that supports Scripting

- Click on the control with the mouse.
- Check taht the scription action executes properly.
- If the congrol is an anchor element, check that the URI in the href attribute on the anchor element is not invoked.
- Check that it is possible to navigate to and give focus to the control via the keyboard.
- Set keyboard focus to the control.
- Check that pressing ENTER invokes the scription action.
- If the control is an anchor element, check that the URI in the href attribute of the anchor element is not invoked.

2. In a user agent that does not supprt Scripting

- Click on the control with the mouse.
- If the control is an anchor element, check that the URI in the href attribute of the anchor element is invoked.
- Check that it is possible to novigate to and give focus to the control via the keyboard.
- Set keyboard focus to the control.
- If the control is an anchor element, check that pressing ENter invoeks the URI of the anchor element's href attribute.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR35)

</details>

<details>
  <summary>What abjective of providing a mechanism to allow users to display moving, scrolling, or auto-updating text in a static window or area?</summary>

Some Web pages display scrolling text because there is limited space available. Scrolling the text in a small text window makes the content available for users who can read quickly enough, but causes problems for users who read more slowly or use assistive technology. This technique provides a mechanism to stop the movement and make the entire block of thext available statically. The text may be made available in a separated window or in a larger section of the page. Users can then read the text at their own speed.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR36)

</details>

<details>
  <summary>What abjective of creating a conforming alternate version for a web page designed with progressive enhancement?</summary>

This objective of this technique is to offer a conforming alternate version for a web page designed with progressive enhancement. The technique demonstrates how to use a scripting technique to accomplish this by:

1. Storing the initial pre-enhanced version of the web page so that it can act as a "conforming alternate version" for any later enhanced versions of the content.
2. Inserting a mechanism into all enhanced versions of the web page which allows a user to revert the content back to the stored pre-enhanced Alternate Version.

**Procedure:**

1. Check enhanced versions of the web page contain a link to the "Conforming Alternate Version".
2. Check tat the alternate version is a conforming alternate version of the original page and that it conforms to WCAG 2.0 at the claimed conformance level.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR38)

</details>

<details>
  <summary>What abjective of making content on focus or hover hoverable, dismissible, and persistent?</summary>

Additional content that is displayed when a user moves the pointer over a trigger or moves the keyboard focus to the trigger (for example, a pop-up) must remain visible to allow users time to read and interact with the content and must allow the user to move the pointer over the additional content.

**Procedure:**

For additional content that appears on hover check that:

1. The pointer can be moved over the additional content without the additional content disappearing.
2. The additional content stays visible and does not automatically close after a time.
3. The content can be closed without moving the pointer way from the trigger. Either by pressing Esc, by pressing another documented keyboard shortcut, or by activating the trigger.

For additional content that appears on focus check that:

1. The additional content stays visible and does not automatically close after a time.
2. The content can be closed without moving the focus way from the trigger. Either by pressing Esc, by pressing another other docuemted keyboard shortcut, or by activating the trigger.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/client-side-script/SCR39)

</details>
