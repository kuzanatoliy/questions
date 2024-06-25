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
