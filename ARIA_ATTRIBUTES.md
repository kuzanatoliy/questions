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

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-errormessage)

</details>

<details>
  <summary>What is aria-expanded element</summary>

There are several widgets that can be expanded and collapsed, including menus, dialogs, and accordion panels. Each of these objects, in turn, has an interactive element that controls their opening and closing. The aria-expanded attribute is applied to this focusable, interactive control that toggles the visibility of the object.

Example:

    <label for="username">Username</label>
    <input id="username" name="username" aria-describedby="username-desc" />
    <button
      aria-expanded="false"
      aria-controls="username-desc"
      aria-label="Help about username"
      type="button">
      <span aria-hidden="true">?</span>
    </button>
    <p id="username-desc" hidden>
      Your username is the name that you use to log in to this service.
    </p>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-expanded)

</details>

<details>
  <summary>What is aria-flowto attribute?</summary>

The global aria-flowto attribute identifies the next element (or elements) in an alternate reading order of content. This allows assistive technology to override the general default of reading in document source order at the user's discretion.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-flowto)

</details>

<details>
  <summary>What is aria-haspopup attribute?</summary>

In ARIA, interactive menus, listboxes, trees, grids, and dialogs that appear on top of other content when triggered to appear are considered "popups". These popups are triggered by one or more interactive elements on the page. The availability and type of popup the interactive element will trigger should be identified with the aria-haspopup state.

- false (default) - The element does not have a popup.
- true - The popup is a menu.
- menu - The popup is a menu.
- listbox - The popup is a listbox.
- tree - The popup is a tree.
- grid - The popup is a grid.
- dialog - The popup is a dialog.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-haspopup)

</details>

<details>
  <summary>What is aria-hidden attribute?</summary>

The aria-hidden state indicates whether the element is exposed to an accessibility API.

- false - The element is exposed to the accessibility API as if it was rendered.
- true - The element is hidden from the accessibility API.
- undefined (default) - The element's hidden state is determined by the user agent based on whether it is rendered.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-hidden)

</details>

<details>
  <summary>What is aria-invalid attribute?</summary>

The aria-invalid attribute is used to indicate that the value entered into an input field is not in a format or a value the application will accept. This may include formats such as email addresses or telephone numbers. aria-invalid can also be used to indicate that a required field is empty.

- grammar - A grammatical error was detected.
- false (default) - There are no detected errors in the value.
- spelling - A spelling error was detected.
- true - The value entered by the user has failed validation.

Example:

    <ul>
      <li>
        <label for="name">Full Name</label>
        <input
          type="text"
          name="name"
          id="name"
          aria-required="true"
          aria-invalid="false"
          onblur="checkValidity('name', ' ', 'Invalid name entered (requires both first and last name)');" />
      </li>
      <li>
        <label for="email">Email Address</label>
        <input
          type="email"
          name="email"
          id="email"
          aria-required="true"
          aria-invalid="false"
          onblur="checkValidity('email', '@', 'Invalid e-mail address');" />
      </li>
    </ul>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-invalid)

</details>

<details>
  <summary>What is aria-keyshortcuts attribute?</summary>

A keyboard shortcut is a series of one or several keys that tells software to perform a pre-programmed action. Keyboard shortcuts enable keyboard users to invoke commands using the keyboard that would otherwise require accessing a menu or using touch or a mouse. The aria-keyshortcuts property defines the keyboard keys that have been implemented to activate or give focus to the element on which the attribute is set.

Value examples:

    aria-keyshortcuts="A"
    aria-keyshortcuts="Shift+Space"
    aria-keyshortcuts="Control+Alt+."
    aria-keyshortcuts="Control+Shift+&#39;"
    aria-keyshortcuts="alt+shift+p control+f"
    aria-keyshortcuts="Meta+C Meta+Shift+C"

Example:

    <a href="#content" aria-keyshortcuts="Alt+Shift+A">Skip to content</a>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-keyshortcuts)

</details>

<details>
  <summary>What is aria-lable attribute?</summary>

Sometimes the default accessible name of an element is missing, or does not accurately describe its contents, and there is no content visible in the DOM that can be associated with the object to give it meaning. A common example is a button containing an SVG or icon font (which you shouldn't be using) without any text.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-label)

</details>

<details>
  <summary>What is aria-labelledby attribute?</summary>

The aria-labelledby property enables authors to reference other elements on the page to define an accessible name. This is useful when using elements that don't have native support for associating elements to provide an accessible name.

Example:

    <span
      role="checkbox"
      aria-checked="false"
      tabindex="0"
      aria-labelledby="tac"></span>
    <span id="tac">I agree to the Terms and Conditions.</span>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-labelledby)

</details>

<details>
  <summary>What is aria-level attribute?</summary>

Levels of hierarchy appear in headings, trees, nested grid, nested tablists, and more. If the DOM ancestry does not accurately represent the level, the aria-level attribute should be used to define the hierarchical level elements within their hierarchical structures. Levels increase with depth. The value for aria-level is an integer greater than or equal to 1.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-level)

</details>

<details>
  <summary>What is aria-live attribute?</summary>

When content changes after initial load, assistive technology (AT) users may not "see" the changes. Some changes are important. Others are not. The aria-live attribute enables developers to inform the user of updates and choose, based on importance and urgency, whether to immediately, proactively, or passively inform AT users of changes to the content.

Values:

- assertive - Indicates that updates to the region have the highest priority and should be presented to the user immediately.
- off (default) - Indicates that updates to the region should not be presented to the user unless the user is currently focused on that region.
- polite - Indicates that updates to the region should be presented at the next graceful opportunity, such as at the end of speaking the current sentence or when the user pauses typing.

Examples:

    <div id="announce" aria-live="polite"></div>

    <div id="announce" aria-live="polite">
      <p>This message is announced.</p>
    </div>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-live)

</details>

<details>
  <summary>What is aria-modal attribute?</summary>

A section of content is "modal" means navigation is limited to the area itself and the background (the ancestors and siblings of the modal) is hidden. Setting aria-modal="true" on dialog and alertdialog role containers indicates the presence of a "modal" element to users of assistive technology, but does not actually make the element modal. The features that make the element actually modal must be implemented by the developer.

    <div id="backdrop" class="no-scroll">
      <div
        role="alertdialog"
        aria-modal="true"
        aria-labelledby="dialog_label"
        aria-describedby="dialog_desc">
        <h2 id="dialog_label">Confirmation</h2>
        <div id="dialog_desc">
          <p>Are you sure you want to delete this file?</p>
        </div>
        <button type="button" onclick="closeDialog(this)">
          No. Close this popup.
        </button>
        <button type="button" onclick="deleteFile(this)">
          Yes. Delete the file.
        </button>
      </div>
    </div>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-modal)

</details>

<details>
  <summary>What is aria-multiline attribute?</summary>

The aria-multiline attribute indicates whether a textbox accepts multiple lines of input or only a single line.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-multiline)

</details>

<details>
  <summary>What is aria-multiselectable attribute?</summary>

The default behavior of selection lists, such as <select>, is to be able to choose only one item or option. By default or by convention, when a user is presented with list from which they must select an item, they assume they can only select a single item unless otherwise notified. The aria-multiselectable attribute is the way to inform assistive technology users that they may select more than one item from the current selectable items if they so choose. Lists and trees are examples of roles that might allow users to select more than one item at a time.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-multiselectable)

</details>

<details>
  <summary>What is aria-orientation attribute?</summary>

It may be important for the user to know the orientation to know how to navigate certain widgets, as orientation impacts the expected behaviors of the left, right, up and down arrows. The aria-orientation attribute is used to indicate to assistive technology users whether an element's orientation is horizontal or vertical, or undefined.

Values:

- horizontal - The element is oriented horizontally.
- undefined (default) - The element's orientation is unknown/ambiguous.
- vertical - The element is oriented vertically.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-orientation)

</details>

<details>
  <summary>What is aria-owns attribute?</summary>

The aria-owns attribute identifies an element (or elements) in order to define a visual, functional, or contextual relationship between a parent and its child elements when the DOM hierarchy cannot be used to represent the relationship.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-owns)

</details>

<details>
  <summary>What is aria-placeholder attribute?</summary>

The aria-placeholder attribute defines a short hint (a word or short phrase) intended to help the user with data entry when a form control has no value. The hint can be a sample value or a brief description of the expected format.

Example:

    <span id="date-of-birth">Birthday</span>
    <div
      contenteditable
      role="textbox"
      aria-labelledby="date-of-birth"
      aria-placeholder="MM-DD-YYYY">
      MM-DD-YYYY
    </div>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-placeholder)

</details>

<details>
  <summary>What is aria-posinset attribute?</summary>

The aria-posinset attribute defines an element's number or position in the current set of listitems or treeitems when not all items are present in the DOM.

Example:

    <h2 id="periodictable">Periodic table of chemical elements</h2>
    <ul role="listbox" aria-labelledby="periodictable">
      <li role="option" aria-setsize="118" aria-posinset="1">Hydrogen</li>
      <li role="option" aria-setsize="118" aria-posinset="3">Lithium</li>
      <li role="option" aria-setsize="118" aria-posinset="11">Sodium</li>
      <li role="option" aria-setsize="118" aria-posinset="19">Potassium</li>
    </ul>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-posinset)

</details>

<details>
  <summary>What is aria-pressed attribute?</summary>

Adding aria-pressed to an element with a role of button turns the button into a toggle button. The aria-pressed attribute is only relevant for toggle buttons. It represents the button's current "pressed" state.

Example:

    <button aria-pressed="false">Pause</button>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-pressed)

</details>

<details>
  <summary>What is aria-readonly attribute?</summary>

When you want to indicate that an interactive element works but is not editable, set aria-readonly="true". This indicates to the user that an interactive element that would normally be focusable and copyable has been placed in a read-only (not disabled) state.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-readonly)

</details>

<details>
  <summary>What is aria-relevant attribute?</summary>

Used in ARIA live regions, the global aria-relevant attribute indicates what notifications the user agent will trigger when the accessibility tree within a live region is modified.

Values:

- additions - Element nodes are added to the accessibility tree within the live region.
- all - Shorthand for additions removals text.
- removals - Text content, a text alternative, or an element node within the live region is removed from the accessibility tree.
- text - Text content or a text alternative is added to any descendant in the accessibility tree of the live region.
- additions text (default) - Element nodes are added to the accessibility tree within the live region AND text content or a text alternative is added to any descendant in the accessibility tree of the live region.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-relevant)

</details>

<details>
  <summary>What is aria-required attribute?</summary>

The aria-required attribute indicates that user input is required on the element before a form may be submitted.

Example:

    <div id="tbLabel">Email Address *</div>
    <div
      role="textbox"
      contenteditable
      aria-labelledby="tblabel"
      aria-required="true"
      id="email1"></div>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-required)

</details>

<details>
  <summary>What is aria-roledescription attribute?</summary>

The aria-roledescription attribute defines a human-readable, author-localized description for the role of an element.

Example:

    <div
      role="article"
      aria-roledescription="slide"
      id="slide"
      aria-labelledby="slideheading">
      <h1 id="slideheading">Quarterly Report</h1>
      <!-- remaining slide contents -->
    </div>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-roledescription)

</details>

<details>
  <summary>What is aria-rowcount attribute?</summary>

Some tables have hundreds, even millions, of rows. Even for tables with fewer rows, loading only a subsection of rows may be a design requirement, improve performance, or improve user experience. When only a subset of rows are loaded, you do need to let all users know that only a subset of the data is being displayed. The aria-rowcount attribute is used to define the total number of rows in a table, grid, or treegrid.

Example:

    <div role="grid" aria-rowcount="24">
      <div role="rowgroup">
        <div role="row" aria-rowindex="1">
          <span role="columnheader">First Name</span>
          <span role="columnheader">Last Name</span>
          <span role="columnheader">Position</span>
        </div>
      </div>
      <div role="rowgroup">
        <div role="row" aria-rowindex="7">
          <span role="gridcell">Morgan</span>
          <span role="gridcell">Brian</span>
          <span role="gridcell">Midfielder</span>
        </div>
        <div role="row" aria-rowindex="8">
          <span role="gridcell">Abby</span>
          <span role="gridcell">Dahlkemper</span>
          <span role="gridcell">Defender</span>
        </div>
        <div role="row" aria-rowindex="9">
          <span role="gridcell">Ashlyn</span>
          <span role="gridcell">Harris</span>
          <span role="gridcell">Goalkeeper</span>
        </div>
      </div>
    </div>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-rowcount)

</details>

<details>
  <summary>What is aria-rowindex attribute?</summary>

The aria-rowindex attribute defines an element's position with respect to the total number of rows within a table, grid, or treegrid.

When only a subset of rows are loaded, you do need to let all users know which subsets of rows are being displayed. The aria-rowindex attribute is used to define the cell or row's row index or position with respect to the total number of rows within a table, grid, or treegrid.

Example:

    <div role="grid" aria-rowcount="24">
      <div role="rowgroup">
        <div role="row" aria-rowindex="1">
          <span role="columnheader">First Name</span>
          <span role="columnheader">Last Name</span>
          <span role="columnheader">Position</span>
        </div>
      </div>
      <div role="rowgroup">
        <div role="row" aria-rowindex="7">
          <span role="gridcell">Morgan</span>
          <span role="gridcell">Brian</span>
          <span role="gridcell">Midfielder</span>
        </div>
        <div role="row" aria-rowindex="8">
          <span role="gridcell">Abby</span>
          <span role="gridcell">Dahlkemper</span>
          <span role="gridcell">Defender</span>
        </div>
        <div role="row" aria-rowindex="9">
          <span role="gridcell">Ashlyn</span>
          <span role="gridcell">Harris</span>
          <span role="gridcell" aria-rowspan="2" aria-rowindex="9">Goalkeeper</span>
        </div>
        <div role="row" aria-rowindex="10">
          <span role="gridcell">Alyssa</span>
          <span role="gridcell">Naeher</span>
        </div>
      </div>
    </div>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-rowindex)

</details>

<details>
  <summary>What is aria-rowindextext attribute?</summary>

When you have a very long table or when you purposefully want to display just a section of a table, not all rows may be present in the DOM. When this happens, we use the aria-rowcount with an integer value to define how many rows the table (or grid) would have if all the rows were present and add the aria-rowindex property on each row and spanning cell to provide information on the row index within that larger table. When the value of aria-rowindex is not meaningful or does not reflect the displayed index, we can also add the aria-rowindextext to provide a human readable text alternative to the aria-rowindex integer value.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-rowindextext)

</details>

<details>
  <summary>What is aria-rowspan attribute?</summary>

The aria-rowspan attribute defines the number of rows spanned by a cell or gridcell within a table, grid, or treegrid.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-rowspan)

</details>

<details>
  <summary>What is aria-selected attribute?</summary>

The aria-selected attribute indicates the current "selected" state for gridcell, option, row and tab roles.

Example:

    <div class="tab-interface">
      <div role="tablist" aria-label="Sample Tabs">
        <span
          role="tab"
          aria-selected="true"
          aria-controls="panel-1"
          id="tab-1"
          tabindex="0">
          First Tab
        </span>
        <span
          role="tab"
          aria-selected="false"
          aria-controls="panel-2"
          id="tab-2"
          tabindex="-1">
          Second Tab
        </span>
        <span
          role="tab"
          aria-selected="false"
          aria-controls="panel-3"
          id="tab-3"
          tabindex="-1">
          Third Tab
        </span>
      </div>
      <div id="panel-1" role="tabpanel" tabindex="0" aria-labelledby="tab-1">
        <p>Content for the first panel</p>
      </div>
      <div id="panel-2" role="tabpanel" tabindex="0" aria-labelledby="tab-2" hidden>
        <p>Content for the second panel</p>
      </div>
      <div id="panel-3" role="tabpanel" tabindex="0" aria-labelledby="tab-3" hidden>
        <p>Content for the third panel</p>
      </div>
    </div>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes/aria-selected)

</details>
