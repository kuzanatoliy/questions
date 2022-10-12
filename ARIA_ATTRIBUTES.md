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

<details>
  <summary>What is aria-colcount attribute?</summary>

The aria-colcount attribute defines the total number of columns in a table, grid, or treegrid when not all columns are present in the DOM.

Example:

    <div role="grid" aria-colcount="6">
      <div role="rowgroup">
        <div role="row">
          <div role="columnheader" aria-colindex="1">First name</div>
          <div role="columnheader" aria-colindex="2">Last name</div>
          <div role="columnheader" aria-colindex="5">City</div>
          <div role="columnheader" aria-colindex="6">Zip</div>
        </div>
      </div>
      <div role="rowgroup">
        <div role="row">
          <div role="gridcell" aria-colindex="1">Debra</div>
          <div role="gridcell" aria-colindex="2">Burks</div>
          <div role="gridcell" aria-colindex="5">New York</div>
          <div role="gridcell" aria-colindex="6">14127</div>
        </div>
      </div>
      …
    </div>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-colcount)

</details>

<details>
  <summary>What is aria-colindex attribute?</summary>

The aria-colindex attribute defines an element's column index or position with respect to the total number of columns within a table, grid, or treegrid.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-colindex)

</details>

<details>
  <summary>What is aria-colindextext attribute?</summary>

The aria-colindextext attribute defines a human readable text alternative of the numeric aria-colindex.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-colindextext)

</details>

<details>
  <summary>What is aria-colspan attribute?</summary>

The aria-colspan attribute defines the number of columns spanned by a cell or gridcell within a table, grid, or treegrid.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-colspan)

</details>

<details>
  <summary>What is aria-controls attribute?</summary>

When an interactive or input control, be it a checkbox, radio button, tab panel, icon, toggles, or other, has an impact on another element in a document or application, the aria-controls attribute should be included to indicate which element or elements the user interface widget controls. The aria-controls attribute identifies the element (or elements) whose contents or presence are controlled by the element on which the attribute is set, regardless of what type of interaction initiates the impacted behavior.

Example:

    <h3 id="tab1" aria-selected="true" aria-controls="panel1" aria-extended = "true" role = "tab" tabindex = "0"> Девушки </ h3>

    <div id="panel1" aria-labelledby="tab1" aria-hidden="false" role="tabpanel">
      <h3 tabindex = "0"> Пожалуйста, выберите свою любимую красавицу ... </ h3>
    </div>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-controls)

</details>

<details>
  <summary>What is aria-current attribute?</summary>

When you have a group of related elements, such as several links in a breadcrumb or steps in a multi-step flow, with one element in the group styled differently from the others to indicate to the sighted user that this is the current element within its group, the aria-current should be used to inform the assistive technology user what has been indicated via styling.

Values:

- page - Represents the current page within a set of pages such as the link to the current document in a breadcrumb.
- step - Represents the current step within a process such as the current step in an enumerated multi step checkout flow .
- location - Represents the current location within an environment or context such as the image that is visually highlighted as the current component of a flow chart.
- date - Represents the current date within a collection of dates such as the current date within a calendar.
- time - Represents the current time within a set of times such as the current time within a timetable.
- true - Represents the current item within a set.
- false (default) - Does not represent the current item within a set.

Examples:

    <nav aria-label="Breadcrumb" class="breadcrumb">
      <ol>
        <li>
          <a href="../../../../../"> Web technology for developers </a>
        </li>
        <li>
          <a href="../../../../"> Accessibility </a>
        </li>
        <li>
          <a href="../../../"> ARIA </a>
        </li>
        <li>
          <a href="../../"> ARIA States and Properties </a>
        </li>
        <li>
          <a href="./" aria-current="page"> ARIA: `aria-current` attribute </a>
        </li>
      </ol>
    </nav>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-current)

</details>

<details>
  <summary>What is aria-describedby attribute?</summary>

The aria-describedby attribute lists the ids of the elements that describe the object. It is used to establish a relationship between widgets or groups and the text that describes them.

Example:

    <button aria-describedby="trash-desc">Move to trash</button>
    …

    <p id="trash-desc">
      Items in the trash will be permanently removed after 30 days.
    </p>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-describedby)

</details>

<details>
  <summary>What is aria-description attribute?</summary>

The global aria-description attribute provides a mechanism for the developer to describe or annotate the current element providing greater context for assistive technology users.

Example:

    <div
      role="application"
      aria-label="calendar"
      aria-description="Game schedule for the Boston Red Sox 2021 Season">
      <h1>Red Sox 2021</h1>
      <div role="grid">…</div>
    </div>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-description)

</details>

<details>
  <summary>What is aria-details attribute?</summary>

The aria-details attribute can be used to provide additional information or complex descriptions to an object. It is used to inform assistive technology users about the content by providing more in-depth information, whether that content is within the current document or a link to additional assets.

Example:

    <p>The <strong>cubic-bezier()<strong> functional notation defines a cubic
      <span role="term" aria-details="bezier bezImg">Bézier curve</span>. As
      these curves are continuous, they are often used to smooth down the start and
      end of the curve and are therefore sometimes called easing functions.
    </p>

    <p role="definition" id="bezier">A <strong>Bézier curve</strong>,
    (Pronounced \ ˈbe-zē-ˌā \)
    <i aria-description="English pronunciation">BEH-zee-ay</i>) is a mathematically
    described curve used in computer graphics and animation. The curve is defined
    by a set of control points with a minimum of two. Web related graphics
    and animations use Cubic Béziers, which are curves with four control
    points P<sub>0</sub>, P<sub>1</sub>, P<sub>2</sub>, and P<sub>3</sub>.
    </p>

    <a href="bezierExplanation.html" id="bezImg"
      aria-label="Explanation of Bézier curve in CSS timing functions">
      <img alt="Animated Bézier curve showing 4 control points." src="bezier.gif">
    </a>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-details)

</details>

<details>
  <summary>What is aria-errormessage attribute?</summary>

When there is a user-created error, you want to let them know it exists and tell them how to fix it. There are two attributes you need to use: set aria-invalid="true" to define the object as being in an error state, then add the aria-errormessage attribute with the value being the id of the element containing the error message text for that object.

Example:

    <p>
      <label for="email">Email address:</label>
      <input
        type="email"
        name="email"
        id="email"
        aria-invalid="true"
        aria-errormessage="err1" />
      <span id="err1" class="errormessage">Error: Enter a valid email address</span>
    </p>

</details>
