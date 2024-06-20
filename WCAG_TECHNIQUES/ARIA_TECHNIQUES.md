# ARIA Techniques

<details>
  <summary>What purpose of using the aria-describedby property to provide a descriptive label for user interface controls?</summary>

The purpose of this technique is to demonstrate how to use the WAI-ARIA aria-describedby property to provide programmatically determined, descriptive information about a user interface element. The aria-describedby property may be used to attach descriptive information to one or more elements through the use of an id reference list. The id reference list contains one or more unique element ids.

**Procedure:**

1. Check that there is a user interface control having an aria-describedby attribute that references one or more elements via unique id.
2. Check that the referenced element or elements provide additional information about the user interface control.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA1)

</details>

<details>
  <summary>What objective of identifying a required field with the aria required property?</summary>

The objective of this technique is to provide programmatic indication that a form field (which shown through presentation to be required) is mandatory for successful submission of a form.

**Procedure:**

1. Check whether the aria-required attribute is present.
2. Check whether the value of the aria-required attribute is the correct required state of the user interface component.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA2)

</details>

<details>
  <summary>What objective of using a WAI-ARIA role to expose the role of a user interface component?</summary>

The objective of this technique is to define the role of an element using the role attribute with one of the non-abstract values defined in the WAI-ARIA Definition of Roles. The WAI-ARIA specification provides an informative description of each role, how it relates to other roles, and the states and properties for each role. When rich internet applications define new user interface widgets, expsing the roles enables users to understand the widget and how to interact with it.

**Procedure:**

1. Check that the value of the role attribute is one of the non-abstract roles from the values defined in the WAI-ARIA specification.
2. Check that the characteristics of the user interface component are described by the role.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA4)

</details>

<details>
  <summary>What objective of using a WAI-ARIA state and property attributes to expose the state of a user interface component?</summary>

The objective of this technique is to use WAI-ARIA state and property attributes to expose the state, properties and values of a user interface components so that they can be read and set by assistive technology, and so that assistive technology is notified of changes to these values.

**Procedure:**

1. Check that the required states and properties for the role are present.
2. Check that no WAI-ARIA states or properties that are neither required, supported, nor inherited are present.
3. Check that the state and property values are updated to reflect the current state when the user interface component changes state.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA5)

</details>

<details>
  <summary>What purpose of using aria-label to provide labels for objects?</summary>

The purpose of this technique is to provide a label for objects that can be read by assistive technology. The aria-label attribute provides the text label for an object, such as a button. When a screen reader encounters the object, the aria-label text is read so that the user will know what it is.

**Procedure:**

1. Examine wheter the text description accurately labels the object or provides a description of its purpose or provides equivalent information.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA6)

</details>

<details>
  <summary>What objective of using aria-labelledby for link purpose?</summary>

With the aria-labelledby attribute, authors can use a visible text element on the page as a lable for a focusable element (a form control or a link). For example, a "read more..." link could be associated with the text of the heading of the preceding section to make the purpose of the link unambiguous.

**Procedure:**

1. Check that each id in the value of the aria labelledby attribute matches an id of a text element used as part of the link purpose.
2. Check that the combined value of the text referenced by the one or more ids in the aria labelledby attribute properly describes the purpose of the link element.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA7)

</details>

<details>
  <summary>What objective of using aria-label for link purpose?</summary>

The objective of this technique is to describe the purpose of a link using the aria-label attribute. The aria-label attribute provides a way to place a descriptive text label on an object, such as a link, when there are no elements visible on the page that describe the object.

**Procedure:**

1. Check that the value of the aria-label attribute properly describes the purpose of the link element.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA8)

</details>

<details>
  <summary>What objective of using aria-labelledby to concatenate a label from several text nodes?</summary>

The aria-labelledby property can be used to provide a name for all visual objects. Applied to inputs, the aria-labelledby property can be used to provide a name to native inputs as well as non-native elements, such as custom thext inputs constructed with div contenteditable="true".

**Procedure:**

1. Check that ids referenced in aria-labelledby are unique and mathc the ids of the text nodes that together provide teh label.
2. Check that the concatenated content of elements referenced by aria-labelledby is descriptive for the purpose of function of the element labeled.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA9)

</details>

<details>
  <summary>What purpose of using aria-labelledby to provide a text alternative for non-text content?</summary>

The purpose of this technique is to provide a short description for an element that can be read by assistive technologies by using the aria-labelledby attribute. The aria-labelledby attribute associates an element with text that is visible elsewhere on the page by using an id reference value that matches the id attribute of the labeling element. Assistive technology such as screen readers use the text of the element identified by the value of the aria-labelledby attribute as the text alternative for the element with the attribute.

**Procedure:**

1. Examine each element where the aria-labelledby attribute is present and the element does not support the alt attribute.
2. Check whetehr the value of the aria-labelledby attribute is the id of an element on the web page.
3. Determine that the text of the element identified by the aria-labelledby attribute accurately labels the element, provides a description of its purpose, or provides equivalent information.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA10)

</details>

<details>
  <summary>What purpose of using ARIA landmarks to identify regions of a page?</summary>

The purpose of this technique is to provide programmatic access to sections of a web page. Landmark roles (or "landmarks") programmatically identify sections of a page. Landmarks help assistive technology (AT) users orient themselves to a page and help them navigate easily to various sections of a page.

**Procedure:**

1. Examine each element with a landmark role.
2. Examine wheter the correct element has been used to mark up content. For example: a navigation role has been used to mark up a section with navigation links, or the main role is used to contain the page's main content.
3. If a landmark region needs to have an accessible name to be exposed as a landmark, check to see that there is an accessible name.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA11)

</details>

<details>
  <summary>What purpose of using role=heading to identify headings?</summary>

The purpose of this technique is to provide a way for Assistive Technologies (AT) to identify a piece of content as a heading Applying role="heading" to an element causes an AT (like a screen reader) to treat it as though it were a heading. The role="heading" property must be paired with the aria-level property to define the heading level.

**Procedure:**

1. Examine each element with the attribute role="heading".
2. Determine whether the content of the element is appropriate as a heading.
3. Determine wheter the aria-level value is the appropriate hierarchical level.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA12)

</details>

<details>
  <summary>What purpose of using aria-labelledby to name regions and landmarks?</summary>

The purpose of this technique is to provide names for regions of a page that can be read by assistive technology. The aria-labelledby attribute provides a way to associate a section of the page marked up as a region or landmarks with text that is on the page that labels it.

**Procedure:**

1. Examine each element with attribute role=region or with a landmark role, where an aria labelledby attribute is also present.
2. Check that the value of the aria labelledby attribute is the id of an element on the page.
3. Check that the text of the element with that id accurately labels the section of the page.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA13)

</details>

<details>
  <summary>What purpose of using aria-label to provide an invisible label where a visible label cannot be used?</summary>

In some situations, elements can be given the attribute aria-label to provide an accessible name for situations when there is no visible label due to a chosen design approach or layout but the context and visual appearance of the control make its purpose clear.

In other situations elements can be given the attribute aria-label to provide an accessible name when the native HTML labeling element is not supported by the control - for example, when a div set to contentEditable is used instead of native form elements such as input type="text" or textarea in order to provide a richer text editing experience.

**Procedure:**

1. Check that the value of the aria-label attribute properly describes the purpose of an element where user inptu is required.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA14)

</details>

<details>
  <summary>What purpose of using aria-describedby to provide descriptions of images?</summary>

The objective of this technique is to provide descriptions of images when a short text alternative does not adequately convey the function or information provided in the object.

**Procedure:**

1. Examine each image element where a aria-describedby attribute is present.
2. Examine whether the aria-describedby attribute programmatically associates an element with its thext description, via the id attribute on the element where the text to be used as the description is found.
3. Examine whether the combined text equivalent and associated text description accurately describe or provide the equivalent purpose to the object.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA15)

</details>

<details>
  <summary>What purpose of using aria-labelledby to provide a name for user interface controls?</summary>

The purpose of this technique is to provide names for user interface controls that can be read by assistive technology. WAI-ARIA provides a way to associate text with a section, drawing, form element, picture, and so on using the aria labelledby. This techniques uses the aria-labelledby attribute to associate a user interface control, such as a form field, with text on the page that labels it.

**Procedure:**

1. Check tat the value of the aria labelledby attribute is the id of an element or a space separated list of ids on the web page.
2. Check that the text of the referenced element or elements accurately labels the user interface control.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA16)

</details>

<details>
  <summary>What purpose of using grouping roles to identify related form controls?</summary>

The objective of this technique is to mark up a set of related controls within a form as a group. Any label associated with the group also seves as a common label or qualifier for individual controls in the group. Assistive technologies can indicate the start and end of the group and the group's label as one navigates into and out of the group. This is a vable alternative for grouping form controls programmatically when the user interface's design makes it difficult to employ the fieldset / legned technique.

**Procedure:**

1. Check that the group of logically related input or select elements are contained within an element with role=group.
2. Check that this group has an accessible name defined using aria-label or aria-labelledby.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA17)

</details>

<details>
  <summary>What purpose of using aria-alertdialog to identify errors?</summary>

The purpose of this technique is to alert people that an input error has occurred. Using role="alertdialog" creates a notification. This notification should be modal with the following characteristics:

- aria-label or aria-labelledby attribute gives the alertdialog and accessible name.
- The alertdialog contains at least one focussable element, and the focus should move to that element when the alertdialog opens.
- The tab order is constrained within the alertdialog whilst it is open.
- When the alertdialog is dismissed, the focus moves back to the position it had before the alertdialog opened, if possible.

**Procedure:**

1. Trigger the error that couses the alertdialog to appear.
2. Determine that the alertdialog contains at least one focusable element, and the focus moves to that element when the alertdialog opens.
3. Determine that the tab order is constrained within the alertdialog while it is open, and when the alertdialog is dismissed, the focus moves back to the position it had before the alertdialog opened, if possible.
4. Examine the element with alertdialog applied.
5. Determine that either the aria-label or aria-labelledby attribute has been correctly used to give the alertdialog an accessible name.
6. Determine that the contents of the alertdialog identifies the input error.
7. Determine wheter contents of the alertdialog suggests how to fix the error.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA18)

</details>

<details>
  <summary>What purpose of using ARIA role=alert or Live Regions to identify Errors?</summary>

The purpose of this technique is to notify Assistive Technologies (AT) when an input error occurs. The aria-live attribute makes it possible for an AT (such as a screen reader) to be notified when error messages are injected into a Live Region container. The content within the aria-live region is automatically read by the AT, without the AT having to focus on the place where the text is displayed.

**Procedure:**

1. Determine that an empty error container role=alert or aria-live=assertive attribute is present in the DOM at page load.
2. Trigger the error that causes the content in the live region to appear or update.
3. Determine that the error message was injected into the already present error container.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA19)

</details>

<details>
  <summary>What purpose of using the region role to identify a region of the page?</summary>

This technique demonstrates how to assign a gemeric region role to a section of a page so that user agents and assistive technologies may be able to programmatically identify it. The region role demarcates a segment of the page that contains content of significance so that it is more readily discoverable and navigable. The generic region should be used when the section cannot be marked up using a standard document landmark role.

**Procedure:**

1. Examine the content and ensure that it is important enough to have an independent landmark.
2. Ensure that a standard landmark role is not appropriate for this content.
3. Check that the region has a programmatically determined name.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA20)

</details>
