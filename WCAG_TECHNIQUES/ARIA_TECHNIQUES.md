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
