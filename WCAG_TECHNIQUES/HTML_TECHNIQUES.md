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
