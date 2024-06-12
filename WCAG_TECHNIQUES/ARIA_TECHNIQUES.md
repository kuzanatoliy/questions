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
