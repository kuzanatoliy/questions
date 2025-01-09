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
