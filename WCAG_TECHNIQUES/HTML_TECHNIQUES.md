# HTML Techniques

<details>
  <summary>What abjective of combining adjacent image and text links for the same resource?</summary>

The objective of this technique is to provide both text and iconic representations of links without making the web page more confusing or difficult for keybaord users or assistive technology users. Since different users finding text and icons more usable, providing both can improve the accessibility of the link.

**Procedure:**

1. Check that every img element contained within the a element has a null value set for its alt attribute.
2. Check that the a element contains an img element that has either a null alt attribute value or a value that supplements the link text and describes the image.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H2)

</details>

<details>
  <summary>What abjective of providing text alternatives for the area elements of image maps?</summary>

The objective of this technique is to provide text alternatives that serve the same purpose as the selectable regions of an image map. An image map is an image divided into selectable regions defined by area elements. Each area is a link to another Web page or another part of the current Web page. The alt attribute of each area element serves the same purpose as the selectable are of the image.

**Procedure:**

1. Check that the area element has an alt attribute.
2. Check that the text alternative specified by the alt attribute serves the same purpose as the part of image map image referenced by teh are element of the image map.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H24)

</details>

<details>
  <summary>What abjective of providing a title using the title element?</summary>

All HTML documents, including those in frames, have a title element in the head section that defines in a simple phrase the purpose of the document. This helps users to orient themselves within the site quickly without having to search for orientation information in the body of the page.

**Procedure:**

1. Examine the source code of the HTML document and check that a non-empty title element appears in the head section.
2. Check that the title element describes the docuemnt.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H25)

</details>

<details>
  <summary>What abjective of providing definitions for abbreviations by using the abbr element?</summary>

The objective of this technique is to provide expansions or definitions for abbreviations by using the abbr element. IT is always appropriate to use abbr element for any abbreviation, including acronyms and initialisms.

**Procedure:**

1. Check that an expansion or definition is provided for each abbreviation via abbr.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H28)

</details>

<details>
  <summary>What abjective of providing link text that describes the purpose of a link for anchor elements?</summary>

The objective of this technique is to describe the purpose of a link by providing descriptive text as the content of the an element. The description lets a user distinguish this link from other links in the Web page and helps the user determine whetehr to follow the link. The URI of the destination is generally not sufficiently descriptive.

**Procedure:**

1. Check that text or a text alternative for non-text content is included in the an element.
2. If an img element is the only content of the a element, check that its text alternative describes the purpose of the link.
3. If the element contains one or more img element(s) and the text alternative of the img element(s) is empty, check that the text of the link describes the purpose of the link.
4. If the a element only contains text, check that the text describes the purpose of the link.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H30)

</details>

<details>
  <summary>What abjective of providing submit buttons?</summary>

The objective of this technique is to provide a mechanism that allows users to explicitly request changes of context. The intended use of a submit button is to generate an HTTP request that submits data entered in a form, so it is an appropriate control to use for causing a change of context.

**Procedure:**

1. Find all forms in the content.
2. For each form, check that it has submit button.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H32)

</details>

<details>
  <summary>What abjective of supplementing link text with the title attribute?</summary>

The objective of this technique is to demonstrate how to use a title attribute on an anchor element to provide additional text describing a link. The title attribute is used to provide additional information to help clarify or further describe the purpose of a link. If the supplementary information provided through the title attribute is something the user should know before following the link, such as a warning, then it should be provided in the link thext rather than in the title attribute.

**Procedure:**

1. For each anchor element that has a title attribute, check that the title attribute together with the link text describes the purpose of the link.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H33)

</details>

<details>
  <summary>What abjective of using a unicode right-to-left mark (RLM) or left-to-right mark (LRM) to mix text direction inline?</summary>

The objective of this technique is to demonstrate how to use Unicode right to left marks and left-to-right marks to override the HTML bidrectional algorithm when it produces undesirable results. This may be necessary, for instance, when placing neutral characters such as spaces or punctuation between different directional text runs. The concepts used in this technique are described in Inline markup and bidirectional text in HTML.

**Procedure:**

1. Examine the source for places where text changes direction.
2. When text changes direction, check whether neutral characters such as spaces or punctuation occur adjacent tot text that is rendered in the non-default direction.
3. When check #2 is true and the HTML bidirectional algorithm would produce the wrong placement of the neutral characters, check whether the neutral characters are followed by Unicode right-to-left or left-to-right marks that cause neutral characters to be placed as part of the preceding characters.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H33)

</details>
