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

<details>
  <summary>What is a menuitemradio role?</summary>

A menuitemradio is checkable menuitem in a set of elements with the same role, only one of which can be checked at a time.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/menuitemradio_role)

</details>

<details>
  <summary>What is a meter role?</summary>

A meter is a graphical display of a numeric value within a defined range. For example, showing battery percentage. A meter is not appropriate for values that do not have a meaningful maximum limit. Meters should not be used to indicate progress (for example loading), this should be communicated with the progress element.

Each element with role="meter" must also have one of the following:

An aria-label attribute.
An aria-labelledby attribute pointing to an element with text that describes the meter.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/meter_role)

</details>

<details>
  <summary>What is a navigation role?</summary>

The navigation role is used to identify major groups of links used for navigating through a website or page content.

    <div role="navigation" aria-label="Main">
      <!-- list of links to main website locations -->
    </div>

This is a website's main navigation.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/navigation_role)

</details>

<details>
  <summary>What is a none role?</summary>

The none role is a synonym for the presentation role; they both remove an element's implicit ARIA semantics from being exposed to the accessibility tree.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/none_role)

</details>

<details>
  <summary>What is a note role?</summary>

The note role can be added to parenthetic or ancillary content if no other native element or other role fits the purpose.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/note_role)

</details>

<details>
  <summary>What is an option role?</summary>

The option role is used to identify selections a user can make in a listbox. These options are similar to the option elements in a select element, but they can contain images.

All selectable options should have aria-selected match their state, true when selected and false when not. If an option is not selectable, aria-selected can be omitted. A disabled option can have aria-disabled="true" and aria-selected="false" to communicate to the user that the option is present, albeit disabled.

The option role is for identifying selectable choices of a listbox. Options must be provided an accessible name. Generally, the accessible name for an option should come from the element's descendant content.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/option_role)

</details>

<details>
  <summary>What is a presentation role?</summary>

The presentation role and its synonym none remove an element's implicit ARIA semantics from being exposed to the accessibility tree.

The content of the element will still be available to assistive technologies; it is only the semantics of the container — and in some instance, required associated descendants — which will no longer expose their mappings to the accessibility API.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/presentation_role)

</details>

<details>
  <summary>What is a progress role?</summary>

The progressbar role defines an element that displays the progress status for tasks that take a long time.

Example:

    <div role="progressbar">
      <h3 role="presentation">Title of my progressbar</h3>
    </div>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/progress_role)

</details>

<details>
  <summary>What is a radio role?</summary>

The radio role is one of a group of checkable radio buttons, in a radiogroup, where no more than a single radio button can be checked at a time.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/radio_role)

</details>

<details>
  <summary>What is a radiogroup role?</summary>

Radio groups are collections describing a set of related radio options. A radiogroup is a type of select list that can only have a single entry, or radio, checked at any one time.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/radiogroup_role)

</details>

<details>
  <summary>What is a range role?</summary>

The range abstract role is a generic type of structure role representing a range of values.

**Note** Don't use it.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/range_role)

</details>

<details>
  <summary>What is a region role?</summary>

The region role is an ARIA landmark role. The region role should be reserved for sections of content sufficiently important that users will likely want to navigate to the section easily and to have it listed in a summary of the page. A region role is a more generic term, and should only be used if the section needing to be identified is not accurately described by one of the other landmark roles, such as banner, main, contentinfo, complementary, or navigation.

Example:

    <div role="region" aria-labelledby="region-heading">
      <h2 id="region-heading">
        This heading's `id` attribute helps this region have an accessible name
      </h2>
      <!-- region content -->
    </div>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/region_role)

</details>

<details>
  <summary>What is a roletype role?</summary>

The roletype role's properties describe the structural and functional purpose of objects that are assigned this role, or "instances". A role is a concept that can be used to understand and operate instances.

**Note** Don't use it

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/roletype_role)

</details>

<details>
  <summary>What is a row role?</summary>

An element with role="row" is a row of cells within a tabular structure. A row contains one or more cells, grid cells or column headers, and possibly a row header, within a grid, table or treegrid, and optionally within a rowgroup.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/row_role)

</details>

<details>
  <summary>What is a rowgroup role?</summary>

An element with role="rowgroup" is a group of rows within a tabular structure. A rowgroup contains one or more rows of cells, grid cells, column headers, or row headers within a grid, table or treegrid.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/rowgroup_role)

</details>

<details>
  <summary>What is a rowheader role?</summary>

An element with role="rowheader" is a cell containing header information for a row within a tabular structure of a grid, table or treegrid.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/rowheader_role)

</details>

<details>
  <summary>What is a scrollbar role?</summary>

A scrollbar is a range that controls what part of a viewport's content is currently visible in the viewport's frame; whether the viewport is a full browser size, an iframe, or any element's block formatting context.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/scrollbar_role)

</details>

<details>
  <summary>What is a serch role?</summary>

The search role is used to identify the search functionality; the section of the page used to search the page, site, or collection of sites.

    <form role="search">
      <!-- search input -->
    </form>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/serch_role)

</details>

<details>
  <summary>What is a serchbox role?</summary>

The searchbox role indicates an element is a type of textbox intended for specifying search criteria.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/serchbox_role)

</details>

<details>
  <summary>What is a section role?</summary>

The section role, an abstract role, is superclass role for renderable structural containment components.

**Note** Don't use it

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/section_role)

</details>

<details>
  <summary>What is a sectionhead role?</summary>

The sectionhead role, an abstract role, is superclass role for labels or summaries of the topic of its related section.

**Note** Don't use it

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/sectionhead_role)

</details>

<details>
  <summary>What is a select role?</summary>

The select role, an abstract role, is superclass role for form widgets that allows the user to make selections from a set of choices.

**Note** Don't use it

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/select_role)

</details>

<details>
  <summary>What is a separator role?</summary>

The separator role indicates the element is a divider that separates and distinguishes sections of content or groups of menuitems. The implicit ARIA role the native thematic break hr element is separator.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/separator_role)

</details>

<details>
  <summary>What is a slider role?</summary>

The slider role is for range input widgets where the user selects a value from within given minimum and maximum values.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/slider_role)

</details>

<details>
  <summary>What is a spinbutton role?</summary>

The spinbutton role indicates that the element is an input widget that restricts its value to a set or range of discrete values. The role also comes with increment and decrement functionality. For example, in a widget that enables users to choose an amount to bet in a game of Texas Holdem, the spinbutton role can allow users to select a number between the minimum and maximum bets in increments, as allowed by the current game rules.

Example:

    <p id="day">Enter the day of the month</p>
    <button type="button" tabindex="-1" aria-label="previous day">˱</button>
    <div
      role="spinbutton"
      tabindex="0"
      aria-valuenow="1"
      aria-valuetext="first"
      aria-valuemin="1"
      aria-valuemax="31"
      aria-labelledby="day">
      1
    </div>
    <button type="button" tabindex="-1" aria-label="next day">˲</button>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/spinbutton_role)

</details>

<details>
  <summary>What is a status role?</summary>

The status role defines a live region containing advisory information for the user that is not important enough to be an alert.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/status_role)

</details>

<details>
  <summary>What is a structure role?</summary>

Structure is a superclass abstract role for document structures, like as document, rowgroup, and sectionhead, that support the accessibility of dynamic web content by helping assistive technologies determine active content versus static document content. Some subclass roles, like section role, are in turn superclasses of other roles.

**Note** Don't use it. Do use HTML and subclass structure roles

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/structure_role)

</details>

<details>
  <summary>What is a suggestion role?</summary>

When you've got a content change that involves an insertion and a deletion, there is no way for a screen reader user to work out if the two are related or not. This is the job of role="suggestion", which should be set on an element wrapping both of them like so:

Example:

    <p>
      Freida's pet is a
      <span role="suggestion">
        <span role="deletion">black Cat called Luna</span>
        <span role="insertion">purple T. Rex called Tiny</span>
      </span>.
    </p>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/suggestion_role)

</details>

<details>
  <summary>What is a switch role?</summary>

The ARIA switch role is functionally identical to the checkbox role, except that instead of representing "checked" and "unchecked" states, which are fairly generic in meaning, the switch role represents the states "on" and "off."

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/suggestion_role)

</details>

<details>
  <summary>What is a tab role?</summary>

An element with the tab role controls the visibility of an associated element with the tabpanel role. The common user experience pattern is a group of visual tabs above, or to the side of, a content area, and selecting a different tab changes the content and makes the selected tab more prominent than the other tabs.

Example:

    <div class="tabs">
      <div role="tablist" aria-label="Sample Tabs">
        <button
          role="tab"
          aria-selected="true"
          aria-controls="panel-1"
          id="tab-1"
          tabindex="0">
          First Tab
        </button>
        <button
          role="tab"
          aria-selected="false"
          aria-controls="panel-2"
          id="tab-2"
          tabindex="-1">
          Second Tab
        </button>
        <button
          role="tab"
          aria-selected="false"
          aria-controls="panel-3"
          id="tab-3"
          tabindex="-1">
          Third Tab
        </button>
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

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/suggestion_role)

</details>

<details>
  <summary>What is a table role?</summary>

The table value of the ARIA role attribute identifies the element containing the role as having a non-interactive table structure containing data arranged in rows and columns, similar to the native table HTML element.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/table_role)

</details>

<details>
  <summary>What is a tablist role?</summary>

The tablist role identifies the element that serves as the container for a set of tabs. The tab content are referred to as tabpanel elements.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/tablist_role)

</details>

<details>
  <summary>What is a term role?</summary>

The term role can be used for a word or phrase with an optional corresponding definition.

Example:

    <p>
      <span role="term">Mansplaining</span>,
      <span role="definition"
        >a portmanteau of "man" and "explain", is the patronizing act of explaining
        without being asked to do so, to someone already learned on the topic, often
        after someone has already explained it</span
      >.
    </p>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/term_role)

</details>

<details>
  <summary>What is a textbox role?</summary>

The textbox role is used to identify an element that allows the input of free-form text. Whenever possible, rather than using this role, use an input element with type="text", for single-line input, or a textarea element for multi-line input.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/textbox_role)

</details>

<details>
  <summary>What is a timer role?</summary>

The timer role indicates to assistive technologies that an element is a numerical counter listing the amount of elapsed time from a starting point or the remaining time until an end point. Assistive technologies will not announce updates to a timer as it has an implicit aria-live value of off.

    <div role="timer" id="eggtimer">0</div>

This defines this div element as a timer with no remaining time.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/timer_role)

</details>

<details>
  <summary>What is a toolbar role?</summary>

A toolbar is a collection of commonly used controls, such as buttons or checkboxes, grouped together in a compact visual form. The toolbar role can be used to communicate the presence and purpose of such a grouping to screen reader users and can help reduce the number of tab stops for keyboard users. Only use the toolbar role to group 3 or more controls.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/toolbar_role)

</details>

<details>
  <summary>What is a tooltip role?</summary>

A tooltip is a contextual text bubble that displays a description for an element that appears on pointer hover or keyboard focus.

Example:

    <label for="password">Password:</label>
    <input aria-describedby="passwordrules" id="password" type="password" />
    <div role="tooltip" id="passwordrules">
      <p>Password Rules:</p>
      <ul>
        <li>Minimum of 8 characters</li>
        <li>
          Include at least one lowercase letter, one uppercase letter, one number
          and one special character
        </li>
        <li>Unique to this website</li>
      </ul>
    </div>

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/tooltip_role)

</details>

<details>
  <summary>What is a tree role?</summary>

A tree is a widget that allows the user to select one or more items from a hierarchically organized collection.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/tree_role)

</details>

<details>
  <summary>What is a treegrid role?</summary>

The treegrid role identifies an element as being grid whose rows can be expanded and collapsed in the same manner as for a tree.

[More >>](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/treegrid_role)

</details>
