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

</details>

<details>
  <summary>What is aria-atomic attribute?</summary>

Live regions are sections of a web page that are updated, whether by user interaction or not, when user focus is elsewhere. As they update outside the user's focus, assistive technologies such as screen readers may not "see" the update to report it to the user.

Values:

- false (default) - present only the changed node or nodes.
- true - present the entire changed region as a whole, including the author-defined label if one exists.

</details>
