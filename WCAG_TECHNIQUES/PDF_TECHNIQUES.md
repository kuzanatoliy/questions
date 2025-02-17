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

<details>
  <summary>What purpose of providing links and link text using the Link annotation and the /Link structure element in PDF documents?</summary>

The purpose of this technique is to show how link text in PDF documents can be marked up to be recognizable by keyboard and assistive technology users. That is, the link information is programmatically available to user agents so that links are recognizable when presented in a different format. This is typically accomplished by using a tool for authoring PDF.

**Procedure:**

1. Read each PDF document with a screen reader, listening to hear that the link is read correctly and that it describes the purpose of the link.
2. Visually scan the tag tree to verify that the link is tagged correctly and the link text is exposed.
3. Use a tool that is capable of showing the /Link entry value to open the PDF document and view the hyperlink and link text.
4. Use a tool that exposes the document through the accessbility API and verify that the link has the correct link text.
5. Tab to each link and check that it can be followed to its target by pressing Enter.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF11)

</details>

<details>
  <summary>What purpose of providing name, role, value information for form fields in PDF documents?</summary>

The purpose of this technique is to ensure that assistive technologies can gather information about and interact with form controls in PDF content.

**Procedure:**

1. For the form control, verify that name, role, and value/state are specified by one of the following:

- Use a screen reader to navigate to the form control and check that it can be activated or that its value can be changed. Verify that the name (tooltip) and role are announced.
- Use a tool capable of showing the form field information to open the PDF doucment and verify that the form control has the correct name, role, value, and state infromation.
- Use a tool that exposes the document through the accessibility API, and verify that the form control has the correct name, role, value, and state infromation.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF12)

</details>

<details>
  <summary>What purpose of providing replacement text using the /Alt entry for links in PDF documents?</summary>

The purpose of this technique is to provide replacement link text via the /Alt entry in the property list for a tag. This is usually not necessary, but in some situations, additional information beyond the visible link text is needed particularly for screen reader users. Screen readers can read visible link text, but replacing the screen text with meaningful alternate text for links in a PDF document can make links more accessible.

**Procedure:**

1. For the hyperlink, verify that the alternate link text is properly coded by one of the following:

- Read the PDF document with a screen reader, listening to hear that the alternate link text is read correctly.
- Use a tool that is capable of showing the /Alt entry to open the PDF document and view the hyperlink and alternate link text.
- Use a tool that exposes the doucment through the accessibility API and verify that the alternate link text is the for the link.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF13)

</details>

<details>
  <summary>What purpose of providing running headers and footers in PDF documents?</summary>

The purpose of this technique is to help users locate themselves in a doucment by providing running headers and footers via pagination artifacts. This is normally accomplished using a tool for authoring PDF.

**Procedure:**

1. Check that running headers and/or footers are provided and contain information to help users locate themselves within the document.
2. If section headers are used in the running header or footer, check that the section header and the running header or footer are consistent.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF14)

</details>

<details>
  <summary>What purpose of providing submit buttons with the submit-form action in PDF forms?</summary>

The purpose of this technique is to provide a mechanism that allows users to explicitly request a change of context using the submit-form action in a PDF form. The intended use of a submit button is to generate an HTTP request that submits data entered in a form, so it is an appropriate control to use for causing a change of context. In PDF documents, submit buttons are normally implemented using a tool for authoring PDF.

**Procedure:**

1. For each page that submits a form, visually verify that the form contains a submit button and check one of the following:

- Tab to the button and check that it submits the form in response to user action to select the button.
- Open the PDF document with a tool that is capable of showing the submit-form action and check that the button action is to submit the form.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF15)

</details>

<details>
  <summary>What purpose of setting the default language using the /Lang entry in the doucment catalog of a PDF document?</summary>

The purpose of this technique is to specify a document's default language by setting the /Lang entry in the document catalog. This is normally accomplished using a tool for authoring PDF.

**Procedure:**

Verify that the default language for the document is correctly specified by applying one of the following:

- Read the PDF document with a screen reader, listening to hear the the text is read in the correct natural language.
- Using a PDF editor, check that the language is set to the default document language.
- Use a tool which is capable of showing the /Lang entry value in the docuemnt catalog to open the PDF document and view the language settings.
- Use a tool that exposes the document through the accessibility API and verify that the language is set to the default language.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF16)

</details>

<details>
  <summary>What purpose of specifying consistent page numbering for PDF documents?</summary>

The purpose of this technique is to help users locate themselves in a doucment by ensuring that the page numbering displayed in the PDF viewer page controls has the same page numbering as the document. For example, Adobe Acrobat Pro and Reader display page numbers in the Page Navigation toolbar. The page number format is specified by the /PageLabels entry in the Doucment Catalog.

**Procedure:**

For every section in the docment that uses a different pagination format, check that the page navigation feature uses the same format used on the document pages:

- Select the pages that begin a new pagination format and visually verify that the same format and page number is shown in the page navigation feature.
- Using a screen reader, check that the page number announced in the page navigation feature is the same as page number announced on the doucment page.
- Using a toll that is capable of showing the /PageLabels entries, open the PDF document and view the entries.
- Use a tool that exposes the doucment through the accessibility API, and verify that the /PageLabels entries are specified correctly.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF17)

</details>

<details>
  <summary>What purpose of specifying the document title using the Title entry in the document information dictionary of a PDF document?</summary>

The purpose of this technique is to show how a descriptive title for a PDF document can be specified for assistive technology by using the /Title entry in the document information dictionary and by setting the DisplayDocTitle flag to True in a viewer preferences dictionary. This is typically accomplished by using a tool for authoring PDF.

**Procedure:**

Verify that the title for the document is correctly specified and displayed in the user agent title bar by applying one of the following:

- Open the PDF document with a screen reader, listening to hear that the doucment title is read correctly.
- Using a PDF editor, check that the docuemtn title is specified. Select the Initial View tab to check that the title will be displayed.
- Use a tool which is capable of showing the /Title entry value in the docuemtn catalog to open the PDF document and view the /Title entry and /DisplayDocTitle flag settings.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF18)

</details>
