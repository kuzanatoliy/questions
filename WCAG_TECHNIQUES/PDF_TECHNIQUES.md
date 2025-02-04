# PDF Techniques

<details>
  <summary>What purpose of applying text alternatives to images with the Alt entry in PDF documents?</summary>

The objective of this technique is to provide text alternatives for images via an /Alt entry in the property list for a Tag. This is normally accomplished using a tool for authoring PDF.

**Procedure:**

1. Verify the images have /Alt entries on an enclosing tag by one of the following:

- Read teh PDF document with a screen reader, listening to hear that the equivalent text is read when tabbing to the non-text object or hearing the alternative text read when reading the content line-by-line.
- Using a PDF editor, check that a text alternative is displayed for each image.
- Use a tool which is capable of showing the /Alt entry value, such as aDesigner, to open the PDF document and view the GUI summary to read the text alternatives for images.
- Use a tool that exposes the document through the accessibility API and verify that images have required text equivalents.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF1)

</details>

<details>
  <summary>What purpose of creating bookmarks in PDF documents?</summary>

The intent of this technique is to make it possible for users to locate content using bookmarks in long documents.

A person with cognitive disabilities may prefer a hierarchical outline that provides an overview of the document rather than reading and traversing through many pages. This is also a conventional means of navigating a document that benefits all users.

**Procedure:**

1. Check that the Bookmarks panel displays bookmarks.
2. Check that the bookmarks link to the correct sections in the document.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF2)

</details>

<details>
  <summary>What purpose of ensuring correct tab and reading order in PDF documents?</summary>

The intent of this technique is to ensure that users can navigate through content in a logical order that is consistent with the meaning of the content. Correct tab and reading order is typically accomplished using a tool for authoring PDF.

**Procedure:**

1. Verify that the content is in the correct reading order by one of the following:

- Read the PDF document with a screen reader or a tool that reads aloud, listening to hear that each element is read in the correct order.
- Use a tool that exposes the document through the accessibility API, and verify that the reading order is correct.

2. Verify that the tab order is correct for focusable content by one of the following:

- Use the tab key to traverse the focus order in the document.
- Use a tool that is capable of showing the page object entry that specifies the tab order setting to open the PDF document and view the setting.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF3)

</details>

<details>
  <summary>What purpose of hiding decorative images with the Artifact tag in PDF documents?</summary>

The purpose of this technique is to show how purely decorative images in PDF documents can be marked so that they can be ignored by Assistive Technology by using the /Artifact tag. This is typically accomplished by using a tool for authoring PDF.

**Procedure:**

1. For an image that is purely decorative, use one of the following to verify that it is marked as an artifact:

- Read the PDF document with a screen reader, listening to hear that the docorative images is not announced when reading the content line-by-line.
- Using a PDF editor, make sure the decorative image is marked as an artifact.
- Reflow the doucment and make sure the decorative image does not appear on the page.
- Use a tool that is capable of showing the /Artifact entry or property list, such as aDesigner, to open the PDF document and verify that decoartive images are marked as artifacts.
- Use a tool that exposes the document through the accessibility API and verify that the decorative image is not exposed through the API.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF4)

</details>

<details>
  <summary>What purpose of indicating required form controls in PDF forms?</summary>

The purpose of this technique is to notify the user when a field that must be completed has not been competed in a PDF form. Required fields are implemented using the /Ff entry in the form field's dictionary. This is normally accomplished using a tool for authoring PDFs.

**Procedure:**

1. Check that the required status is indicated in the form contrl's label.
2. Leave the fields blank and submit the form. Check that an alert describing the error is provided.
3. Use a tool that exposes the document through the accessibility API and verify that the required property is indicated.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF5)

</details>

<details>
  <summary>What purpose of using table elements for table markup in PDF Documents?</summary>

The purpose of this technique is to show how tables in PDF documents can be marked up so that they are recognized by assistive technology. This is typically accomplished by using a tool for authoring PDF.

**Procedure:**

1. For each table, confirm one of the following:

- Read the PDF document with a screen reader, listening to hear that the tabular information is presented in a way that preserves logical relationships among the table header and data cells.
- Using a PDF editor, verify that the appropriate TR, TH, and TD tags are in the proper reading order and hierarchy in the table tree.
- Use a tool which is capable of showing the table elements to open the PDF document, view the table structure, and verify that it contains the approproate TR, TH, TD structures.
- Use a tool that exposes the document through the accessibility API, and verify that the table structure contains the appropriate TR, TH, and TD structures, and that they are in the proper reading order and hierarchy.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF5)

</details>
