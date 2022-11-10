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
