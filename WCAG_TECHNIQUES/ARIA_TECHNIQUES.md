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
