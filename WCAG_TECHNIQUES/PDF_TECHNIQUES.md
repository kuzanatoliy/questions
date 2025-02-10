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

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF6)

</details>

<details>
  <summary>What purpose of performing OCR on a scanned PDF document to provide actual text?</summary>

The purpose of this technique is to ensure that visually rendered text is presented in such a manner that it can be perceived without its visual presntation interfering with its readability.

**Procedure:**

For each page converted to text using OCR, ensure that the resulting PDF has been converted correctly, using one of the following ways:

1. Read teh PDF document with a screen reader or a tool that reads aloud listening to hear that all text is read correctly and in the correct reading order.
2. Save the document as text and check that the converted text is complete and in the correct reading order.
3. Use a tool that is capable of showing the converted content to open the PDF document and verify that all text was converted and is in the correct reading order.
4. Use a tool that exposes the document through the accessibility API and verify that all text was converted and is in the correct reading order.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF7)

</details>

<details>
  <summary>What purpose of providing definitions for abbreviations via an E entry for a strcuture element?</summary>

The purpose of this technique is to provide an expansion or definition of an abbreviation for the first occurrence of the abbreviation. For example, a reference to an abbreviation, such as "WCAG", should be available as "Web Content Accessibility Guidelines (WCAG)" on its first occurrence in a document.

**Procedure:**

Verify that the first occurrence of abbreviations that require expansion text have /E entries on an enclosing tag by one of the following and that both the abbreviation and the expansion text are provided:

- In a PDF editor, locate the tag for the text that is the abbreviation, and check that an expansion or definition is provided for each abbreviaotion in the Expansion Text field in the corresponding tag's properties.
- Read the PDF document with a screen reader, listening to hear that on the first occurence, the abbreviation and expansion are read when the screen reader reads the content line-by-line.
- Use a tool that is capable of showing the /E entry value, such as aDesigner to open the PDF document and view the GUI summary to read the text expansions for abbreviations.
- Use a tool that exposes the document through the accessibility API and verify that the text expaonsion of the abbreviation is properly implemented.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF8)

</details>

<details>
  <summary>What purpose of providing headings by marking content with heading tags in PDF documents?</summary>

The purpose of this technique is to show how headings in PDF documents can be marked so that they are recognized by assistive technologies. Headings are marked up using the heading elements (H, H1, H2, ... H6) in the structure tree. This is typically accomplished by using a tool for authoring PDF.

**Procedure:**

For all PDF content that is divied into separate sections, use one of the following to verify that headings are tagged correctly:

- Read the PDF document with a screen reader, listening to hear that the list of headings is announced correctly.
- Using a PDF editor, make sure that headings are tagged correctly.
- Use a tool that is capable of showing the /Headn entries to open the PDF document and verify that headings are tagged correctly.
- Use a tool that exposes the document through the accessibility API and verify that the headings are tagged correctly.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF9)

</details>

<details>
  <summary>What purpose of providing labels for interactive form controls in PDF documents?</summary>

The purpose of this technique is to ensure that users of assistive technology are able to perceive form control labels and understand how form controls are used.

**Procedure:**

1. For each form control, verify visually that the label is positioned correctly in relation to the control.
2. For each form control, verify that the name is programmatically associated with the control by one of the following:

- Open the PDF document with a tool that is capable of showing the name assocaited with the control and verify that the name is assocaited correctly with the control.
- Use a tool that exposes the document through the accessibility API, and verify that the name is associated correctly with the control.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF10)

</details>
