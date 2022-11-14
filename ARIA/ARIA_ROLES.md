# Aria Roles

<details>
  <summary>What are aria roles?</summary>

ARIA roles provide semantic meaning to content, allowing screen readers and other tools to present and support interaction with object in a way that is consistent with user expectations of that type of object. ARIA roles can be used to describe elements that don't natively exist in HTML or exist but don't yet have full browser support.

</details>

<details>
  <summary>What is an alert role?</summary>

The alert role is used to communicate an important and usually time-sensitive message to the user. When this role is added to an element, the browser will send out an accessible alert event to assistive technology products which can then notify the user.

The alert role should only be used for information that requires the user's immediate attention, for example:

- An invalid value was entered into a form field
- The user's login session is about to expire
- The connection to the server was lost so local changes will not be saved

**Note** It is possible to use aria-live="alert" instead of the role.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/alert_role)

</details>

<details>
  <summary>What is an alertdialog role?</summary>

The alertdialog role is used to notify users of urgent information that demands the user's immediate attention. Including role="alertdialog" on the element containing the dialog helps assistive technology identify the content as being grouped and separated from the rest of the page content. Examples include error messages that require confirmation and other action confirmation prompts.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/alertdialog_role)

</details>

<details>
  <summary>What is an application role?</summary>

The application document structure role, indicates to assistive technologies that this part of the web content contains elements that do not conform to any other known HTML element or WAI-ARIA widget. Any sort of special interpretation of HTML structures and widgets should be suspended, and control should be completely handed over to the browser and web application to handle mouse, keyboard, or touch interaction.

In this mode, the web author is completely responsible for handling any and all keyboard input, focus management, and other interactions and cannot assume assistive technologies would do any processing on their end.

If the web application encompassed by the application role contains parts that should be treated like normal web content, a role of document or article should be used to contain such content.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/application_role)

</details>

<details>
  <summary>What is an article role?</summary>

The article document structure role denotes a section of a document, page, or site that, if it were standing on its own, could be viewed as a complete document, page or site. The aim of a set of article sections is to indicate their relationship to one another.

**Note** It is possible to use article tag instead of the role.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/article_role)

</details>

<details>
  <summary>What is a banner role?</summary>

A banner landmark role overwrites the implicit ARIA role of the container element upon which it is applied. It should be reserved for globally repeating site-wide content that is generally located at the top of every page.

**Note** It is possible to use header tag instead of the role.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/banner_role)

</details>

<details>
  <summary>What is a button role?</summary>

The button role identifies an element as a button to assistive technology such as screen readers. A button is a widget used to perform actions such as submitting a form, opening a dialog, canceling an action, or performing a command such as inserting a new record or displaying information. Adding role="button" tells assistive technology that the element is a button but provides no button functionality. Use <button> or <input> with type="button" instead.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/button_role)

</details>

<details>
  <summary>What is a ceil role?</summary>

The element with role="cell" is a cell within a row, optionally within a rowgroup, within a table. If the cell is in a grid or treegrid, opt for gridcell. Using native HTML td elements, whenever possible, is strongly encouraged.

Each element with role="cell" MUST be nested in a container element with role="row". That row, in turn, can be nested within an element with role="rowgroup", and should be nested within a grid, table or treegrid. If a cell contains column or row header information, use the columnheader or rowheader roles, respectively. If the cell does not contain header information and is nested in a grid or treegrid, the role of gridcell may be more appropriate.

A cell can contain a number of property attributes clarifying the cell's position within the tabular data structure, including aria-colindex, aria-colspan, aria-rowindex, and aria-rowspan.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/cell_role)
.

</details>

<details>
  <summary>What is a checkbox role?</summary>

The native HTML checkbox form control had two states ("checked" or "not checked"), with an indeterminate state settable via JavaScript. Similarly, an element with role="checkbox" can expose three states through the aria-checked attribute: true, false, or mixed.

Since a checkbox is an interactive control, it must be focusable and keyboard accessible. If the role is applied to a non-focusable element, use the tabindex attribute to change this. The expected keyboard shortcut for activating a checkbox is the Space key.

The developer is required to change the value of the aria-checked attribute dynamically when the checkbox is activated.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/checkbox_role)

</details>

<details>
  <summary>What is columnheader role?</summary>

An element with role="columnheader" nested as a descendant for an element with role="row", is a static tabular structure of a column header cell in a tabular container, either a table or grid, or other chart that needs to show data relationships. To be supported, the columnheader must be nested in an element with the role of row.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/columnheader_role)

</details>

<details>
  <summary>What is a combobox role?</summary>

A combobox is a composite widget that combines a named input field with a popup providing possible values for that input field. The purpose of a this widget is to improve user experience by helping the user select a value without having to type in the complete value and, optionally depending whether supported values are limited, preventing the user from entering invalid or otherwise unsupported values.

The combobox role is set on input that controls another element, such as a listbox or grid, that can dynamically pop up to help the user set the value of the input.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/combobox_role)

</details>

<details>
  <summary>What is a command role?</summary>

The command role defines a widget that performs an action but does not receive input data.

**note** don't use it.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/command_role)

</details>

<details>
  <summary>What is a comment role?</summary>

The comment landmark role semantically denotes a comment/reaction to some content on the page, or to a previous comment.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/comment_role)

</details>

<details>
  <summary>What is a complementary role?</summary>

The complementary landmark role is used to designate a supporting section that relates to the main content, yet can stand alone when separated. These sections are frequently presented as sidebars or call-out boxes. If possible, use the HTML aside element instead.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/complementary_role)

</details>

<details>
  <summary>What is a composite role?</summary>

The composite abstract role indicates a widget that may contain navigable descendants or owned children.

**note** don't use it.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/composite_role)

</details>

<details>
  <summary>What is a contentinfo role?</summary>

The contentinfo role defines a footer, containing identifying information such as copyright information, navigation links, and privacy statements, found on every document within a site. This section is commonly called a footer.

**note** use footer tag instead of the contentinfo role

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/contentinfo_role)

</details>

<details>
  <summary>What is a definition role?</summary>

The definition ARIA role can be included an element that is a definition of a term or concept, similar to the native dfn element. To associate the definition with the term being defined, and to provide an accessible name, reference the term being defined with role="term", using aria-labelledby.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/definition_role)

</details>

<details>
  <summary>What is a dialog role?</summary>

The dialog role is used to mark up an HTML based application dialog or window that separates content or UI from the rest of the web application or page. Dialogs are generally placed on top of the rest of the page content using an overlay. Dialogs can be either non-modal (it's still possible to interact with content outside of the dialog) or modal (only the content in the dialog can be interacted with).

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/dialog_role)

</details>

<details>
  <summary>What is a document role?</summary>

The document role is for the top container containing content that assistive technology users may want to browse in a reading mode. Only useful on focusable sections within complex composite widgets or applications, the document role inform assistive technologies to the reading context back to a reading mode: The document role tells assistive technologies with reading or browse modes to use the document mode to read the content contained within this element.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/document_role)

<details>

<details>
  <summary>Waht are structural roles?</summary>

Structural ARIA roles were originally created as a bridge to inform assistive technologies of HTML5 elements that were not yet fully supported in browsers. Some roles, like presentation, toolbar and tooltip, provide information on the document structure to assistive technologies in cases where equivalent native HTML elements don't exist. Other roles, including those listed in the table below, are not needed, as there are semantic HTML elements with the same meanings. In many cases, these equivalent HTML elements have always been supported.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/structural_roles)

</details>

<details>
  <summary>What is a feed role?</summary>

A feed is a dynamic scrollable list of articles in which articles are added to or removed from either end of the list as the user scrolls. A feed enables screen readers to use the browse mode reading cursor to both read and scroll through a stream of rich content that may continue scrolling infinitely by loading more content as the user reads.

Example:

    <section role="feed" aria-busy="false">
      …
      <article aria-posinset="427" aria-setsize="-1">…</article>
      <article aria-posinset="428" aria-setsize="-1">…</article>
      <article aria-posinset="429" aria-setsize="-1">…</article>
      …
    </section>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/feed_role)

</details>

<details>
  <summary>What is a figure role?</summary>

A figure is a perceivable section of content that typically contains a graphical document, images, code snippets, or example text. The parts of a figure MAY be user-navigable. Any content that should be grouped together and consumed as a figure (which could include images, video, audio, code snippets, or other content) can be identified as a figure using role="figure".

Example:

    <div role="figure" aria-labelledby="caption">
      <img src="image.png" alt="put image description here" />
      <p id="caption">Figure 1: The caption</p>
    </div>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/figure_role)

</details>

<details>
  <summary>What is a form role?</summary>

The form role can be used to identify a group of elements on a page that provide equivalent functionality to an HTML form.

Example:

    <div role="form" id="contact-info" aria-label="Contact information">
      <!-- form content -->
    </div>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/form_role)

</details>

<details>
  <summary>What is a generic role?</summary>

While ARIA is primarily used to express semantics, there are some elements that shouldn't expose a semantic name to assistive technologies. The generic role indicates an element's role is equivalent to that of the non-semantic div and span elements.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/generic_role)

</details>

<details>
  <summary>What is a grid role?</summary>

The grid role is a composite widget containing a collection of one or more rows with one or more cells where some or all cells in the grid are focusable by using methods of two-dimensional navigation, such as directional arrow keys.

Example:

    <table role="grid" aria-labelledby="id-select-your-seat">
      <caption id="id-select-your-seat">
        Select your seat
      </caption>
      <tbody role="presentation">
        <tr role="presentation">
          <td></td>
          <th>Row A</th>
          <th>Row B</th>
        </tr>
        <tr>
          <th scope="row">Aisle 1</th>
          <td tabindex="0">
            <button id="1a" tabindex="-1">1A</button>
          </td>
          <td tabindex="-1">
            <button id="1b" tabindex="-1">1B</button>
          </td>
          <!-- More Columns -->
        </tr>
        <tr>
          <th scope="row">Aisle 2</th>
          <td tabindex="-1">
            <button id="2a" tabindex="-1">2A</button>
          </td>
          <td tabindex="-1">
            <button id="2b" tabindex="-1">2B</button>
          </td>
          <!-- More Columns -->
        </tr>
      </tbody>
    </table>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/grid_role)

</details>

<details>
  <summary>What is a gridcell role?</summary>

The gridcell role is used to make a cell in a grid or treegrid. It is intended to mimic the functionality of the HTML <td> element for table-style grouping of information.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/gridcell_role)

</details>

<details>
  <summary>What is a group role?</summary>

The group role identifies a set of user interface objects that is not intended to be included in a page summary or table of contents by assistive technologies.

    <div role="menu">
      <ul role="group">
        <li role="menuitem">Inbox</li>
        <li role="menuitem">Archive</li>
        <li role="menuitem">Trash</li>
      </ul>
      <ul role="group">
        <li role="menuitem">Custom Folder 1</li>
        <li role="menuitem">Custom Folder 2</li>
        <li role="menuitem">Custom Folder 3</li>
      </ul>
      <ul role="group">
        <li role="menuitem">New Folder</li>
      </ul>
    </div>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/group_role)

</details>

<details>
  <summary>What is a heading role?</summary>

The heading role defines this element as a heading to a page or section, with the aria-level attribute providing for more structure.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/heading_role)

</details>

<details>
  <summary>What is an img role?</summary>

The ARIA img role can be used to identify multiple elements inside page content that should be considered as a single image. These elements could be images, code snippets, text, emojis, or other content that can be combined to deliver information in a visual manner.

Example:

    <div role="img" aria-label="Description of the overall image">
      <img src="graphic1.png" alt="" />
      <img src="graphic2.png" />
    </div>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/img_role)

</details>

<details>
  <summary>What is an input role?</summary>

The input role is an abstract role. It must not be used by web authors. It is the superclass for input widgets that provide for user input, including checkbox, radio, and textbox. For all three, consider using the input element of type checkbox, radio and text, respectively.

**Note** Don't use it.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/input_role)

</details>

<details>
  <summary>What is a landmark role?</summary>

A landmark is an important subsection of a page. The landmark role is an abstract superclass for the aria role values for sections of content that are important enough that users will likely want to be able to navigate directly to them.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/landmark_role)

</details>

<details>
  <summary>What is a link role?</summary>

A link widget provides an interactive reference to a resource. The target resource can be either external or local; i.e., either outside or within the current page or application.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/link_role)

</details>

<details>
  <summary>What is a list role?</summary>

Any content that consists of an outer container with a list of elements inside it can be identified to assistive technologies using the list and listitem containers respectively. A list must have one or more listitem children, or, alternatively, have one or more groups as children, with each group having one or more listitems as children.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/list_role)

</details>

<details>
  <summary>What is a listbox role?</summary>

The listbox role is used to identify an element that creates a list from which a user may select one or more static items, similar to the HTML select element. Unlike select, a listbox can contain images. Each child of a listbox should have a role of option.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/listbox_role)

</details>

<details>
  <summary>what is a listitem role?</summary>

Any content that consists of an outer container with a list of elements inside it can be identified to assistive technologies using the list and listitem containers respectively.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/listitem_role)

</details>

<details>
  <summary>what is a log role?</summary>

The log role is used to identify an element that creates a live region where new information is added in a meaningful order and old information may disappear.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/log_role)

</details>

<details>
  <summary>What is a main role?</summary>

The main landmark role is used to indicate the primary content of a document. The main content area consists of content that is directly related to or expands upon the central topic of a document, or the main function of an application.

    <div id="main" role="main">
      <h1>Avocados</h1>
      <!-- main section content -->
    </div>

This is the main section of a document that discusses avocados. Subsections of this document could discuss their history, the different types, regions where they grow, etc.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/main_role)

</details>

<details>
  <summary>What is a mark role?</summary>

The mark role semantically denotes HTML elements containing text that is marked/highlighted for reference purposes. This is semantically equivalent to the HTML mark element. If possible, you should use this element instead.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/mark_role)

</details>

<details>
  <summary>What is a marquee role?</summary>

The marquee role defines an area as a type of live region that presents non-essential information that changes frequently. Examples of marquees include stock tickers and ad banners; information that is not necessarily sought out by the user that may be presented in any order. The main difference between a marquee and a log is that log information is presented in a meaningful order such as a by date.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/marquee_role)

</details>

<details>
  <summary>What is a math role?</summary>

The math role indicates that the content represents a mathematical expression.

Examples:

    <div role="math" aria-label="a^{2} + b^{2} = c^{2}">
      a<sup>2</sup> + b<sup>2</sup> = c<sup>2</sup>
    </div>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/math_role)

</details>

<details>
  <summary>What is a menu role?</summary>

A menu generally represents a grouping of common actions or functions that the user can invoke. The menu role is appropriate when a list of menu items is presented in a manner similar to a menu on a desktop application. Submenus, also known as pop-up menus, also have the role menu.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/menu_role)

</details>

<details>
  <summary>What is a menubar role?</summary>

The menubar role is used to create a menu bar similar to those found near the top of the window in many desktop applications, visually persistent, typically horizontal, bar of menu items offering the user quick access to a consistent set of commands.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/menubar_role)

</details>

<details>
  <summary>What is a menuitem role?</summary>

A menuitem is one of the three types of options in a set of choices contained by a menu or menubar; the other two being menuitemcheckbox and menuitemradio. The menuitem is only found as a descendant of, or owned by, elements with role menu or menubar, optionally nested within an element with role group that is contained in, or owned by, a menu.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/menuitem_role)

</details>

<details>
  <summary>What is a menuitemcheckbox role?</summary>

A menuitemcheckbox is a menuitem with a checkable state whose possible values are true, false, or mixed.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/menuitemcheckbox_role)

</details>
