# Aria Attributes

<details>
  <summary>What is aria-activedescendant attribute?</summary>

The aria-activedescendant property provides a method of managing focus for assistive technologies on interactive elements when they contain multiple focusable descendants, such as menus, grids, and toolbars. Instead of the screen reader moving focus between owned elements, aria-activedescendant can be used on container elements to refer to the currently active element, informing assistive technology users of the currently active element when focused.

This attribute is only relevant on elements with role of composite widget, combobox, textbox, group, or application whose id is referenced as the attribute value.

Example:

    <div role="toolbar" tabindex="0" aria-activedescendant="button1">
      <img src="btncut.png" id="button1" role="button" alt="cut" />
      <img src="btncopy.png" id="button2" role="button" alt="copy" />
      <img src="btnpaste.png" id="button3" role="button" alt="paste" />
    </div>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-activedescendant)

</details>

<details>
  <summary>What is aria-atomic attribute?</summary>

Live regions are sections of a web page that are updated, whether by user interaction or not, when user focus is elsewhere. As they update outside the user's focus, assistive technologies such as screen readers may not "see" the update to report it to the user.

Values:

- false (default) - present only the changed node or nodes.
- true - present the entire changed region as a whole, including the author-defined label if one exists.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-atomic)

</details>

<details>
  <summary>What is aria-autocomplete attribute?</summary>

The aria-autocomplete attribute indicates whether inputting text could trigger display of one or more predictions of the user's intended value for a combobox, searchbox, or textbox and specifies how predictions will be presented if they are made.

Values:

- none (default) - When a user is providing input, not automatic suggestion is displayed.
- inline - aria-autocomplete="inline" text suggesting one way to complete the provided input may be dynamically inserted after the caret.
- list - aria-autocomplete="list" When a user is providing input, an element containing a collection of values that could complete the provided input may be displayed.
- both - aria-autocomplete="both" an input to offer both models at the same time. When a user is providing input, an element containing a collection of values that could complete the provided input may be displayed. If displayed, one value in the collection is automatically selected, and the text needed to complete the automatically selected value appears after the caret in the input.

Example:

    <input id="cb1-edit" class="cb_edit" type="text" tabindex="0" role="combobox" aria-autocomplete="inline" aria-owns="list" />
    <ul id="list" tabindex="-1" role="listbox" aria-expanded="true">
      <li id ​​= "cb1-opt1" role = "option"> Qingchuan </ li>
      <li id ​​= "cb1-opt2" role = "option"> Цзин Цю </ li>
      <li id ​​= "cb1-opt3" role = "option"> Хуан Сяосянь </ li>
    </ul>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-autocomplete)

</details>

<details>
  <summary>What is aria-braillelabel attribute?</summary>

The global aria-braillelabel attribute is similar to the global aria-label in that it defines a string value that labels the current element. While aria-label is read by the screen reader, the contents of the aria-braillelabel attribute are converted into Braille; providing the user with a recognizable name of the object in Braille.

Example:

    <button aria-braillelabel="***">
      <img alt="3 out of 5 stars" src="three_stars.png" />
    </button>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-braillelabel)

</details>

<details>
  <summary>What is aria-brailleroledescription attribute?</summary>

The global aria-brailleroledescription attribute defines a human-readable, author-localized abbreviated description for the role of an element intended to be converted into Braille.

Example:

    <article
      aria-roledescription="slide"
      aria-brailleroledescription="sld"
      aria-labelledby="slide1heading">
      <h1 id="slide1heading">Welcome to my talk</h1>
      <img alt="Me" src="images/me.jpg" />
    </article>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-brailleroledescription)

</details>

<details>
  <summary>What is aria-busy attribute?</summary>

Used in ARIA live regions, the global aria-busy state indicates an element is being modified and that assistive technologies may want to wait until the changes are complete before informing the user about the update.

When multiple parts of a live region need to be loaded before changes are announced to the user, set aria-busy="true" until loading is complete. Then set to aria-busy="false". This prevents assistive technologies from announcing changes before updates are done.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-busy)

</details>

<details>
  <summary>What is aria-checked attribute?</summary>

The aria-checked attribute indicates the current "checked" state of checkboxes, radio buttons, and other widgets.

Values:

- false - the element supports being checked but is not currently checked.
- true - the element is checked.
- mixed - for checkbox and menuitemcheckbox only, equivalent to indeterminate, indicating a mixed mode value of neither checked nor unchecked.
- undefined (default) - the element does not support being checked.

Example:

    <span
      role="checkbox"
      id="checkBoxInput"
      aria-checked="false"
      tabindex="0"
      aria-labelledby="chk15-label"></span>
    <label id="chk15-label">Subscribe to the newsletter</label>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-checked)

</details>
