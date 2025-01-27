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

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H34)

</details>

<details>
  <summary>What abjective of using alt attributes on images used as submit buttons?</summary>

For input elements of type image, the alt attribute of the input element is used to provide a functional label. This label indicates the button's function, but does not attempt to describe the image. This label indicates the button's function, but does not attempt to describe the image. The label is especially important if there are multiple submit buttons on the page that each lead to different results.

**Procedure:**

1. For all input elements that have a type attribute value of image, check for the presence of an alt attribute.
2. Check that the value of the alt attribute describes the button's function.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H36)

</details>

<details>
  <summary>What abjective of using alt attributes on img elements?</summary>

When using the img element, specify a short text alternative with the alt attribute. Note. The value of this attribute is referred to as "alt text".

When an image contains words that are important to understanding the content, the alt text should inculde those words. This will allow the alt text to play the same function on the page as the image. Note that it does not necessarily describe the visual characterisics of the image itself but must convey the same meaning as the image.

**Procedure:**

1. Examine each img element in the content.
2. Check that each img element which conveys meaning contains an alt attribute.
3. If the image contains words that are important to understanding the content, the words are included int the text alternative.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H37)

</details>

<details>
  <summary>What abjective of using caption elements to associate data table captions with data tables?</summary>

The objective of this technique is to programmatically associate captions for data tables where captions are provided in the presentation. The caption for a table is a table identifier and acts like a title or heading for the table.

**Procedure:**

1. Check that the table includes a caption element.
2. Check that the text that titles or describes the table is included in hte caption element.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H39)

</details>

<details>
  <summary>What abjective of using description lists?</summary>

The objective of this technique is to provide the description of names or terms by presentiong them in a description list. The list is marked up using the dl element. Within the list, each term is put in a separate dt element, and its description goes in the dd element directly following it. Multiple terms can be associated with a single description, as can a single term with multiple descriptions, provided that semantic sequence is maintained. The title attribute can be used to provide additional information about the description list. Usage of description lists ensures that temrs and their desctions are semantically related even as presentaion format changes, as well as ensuring that these terms and desctions are semantically grouped as a unit.

**Procedure:**

1. Check that the list is contained within a dl element.
2. Check that each term in the list being described is contained iwthin a dt element.
3. Check that when there is more than one term that shares the same description that the dt elements immediately follow each other.
4. Check that the description for each term is contained in one or more dd elements.
5. Check that the one or more dd elements immediately follow the one or more dt elements containing the term being described.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H40)

</details>

<details>
  <summary>What abjective of using h1-h6 to identify headings?</summary>

The objective of this technique is to use HTML heading markup to provide semantic code for headings in the content. Heading markup will allow assistive technologies to present the heading status of text to a user. A screen reader can recognize the code and announce the text as a heading with its level, beep or provide some other auditory indicator. Screen readers are also able to navigate heading markup which can be an effective way for screen reader users to more quickly find the content of interest. Assistive technologies that alter the authored visual display will also be able to provide and appropriate alterante visual display for headings that can be identified by heading markup.

**Procedure:**

1. Check that heading markup is used when content is a heading and the heading markup indicates the appropriate heading level for the content.
2. Check that heading markup is not used when content is not a heading.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H42)

</details>

<details>
  <summary>What abjective of using id and headers attributes to associate data cells with header cells in data tables?</summary>

The objective of this technique is to associate each data cell with the appropriate headers. This technique adds a headers attribute to each data cell. It also adds an id attribute to any cell used as a header for other cells. The headers attribute of a cell contains a list of the id attributes of the associated header cells. If there is more than one id, they are separated by spaces.

**Procedure:**

1. Check for layout tables: determine whether the content has a relationship with other content in both its column and its row. If "no", the table is a layout table. If "yes", the table is a data table.
2. For data tables, check that any cell that is associated with more than one row and/or one column header contains a headers attribute that list the id for all headers associated with that cell.
3. For data tables where any cell contains an id or headers attribute:

- Checka that each id listed in the headers attribute of the data cell matches the id attribute of a cell that is used as a header element.
- Check that the headers attribute of a data cell contains the id attribute of all headers associated with the data cell.
- Check that all ids are unique.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H43)

</details>

<details>
  <summary>What abjective of using label elements to associate text labels with form controls?</summary>

The objective of this technique is to use the label element to explicitly associate a form control with a label. A label is attached to a specific form control through the use of the for attribute. The value of the for attribute must be the same as the value of the id attribute of the form control.

**Procedure:**

- For all input elements of type text, file or password, for all texterea elements, and for all select elements in the Web page:

1. Check that there is a label element that identifies the purpose of the control before the input, textarea, or select element.
2. Check that the for attribute of the label element matches the id of the input, textarea, or select element.
3. Check that the albel element is visible.

- For all input elements of type checkbox or radio in the Wb page:

1. Check that there is a label element that identifies the purpose of the control after the input element.
2. Check that the for attribute of the label element matches the id of the input element.
3. Check that the label element is visible.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H44)

</details>

<details>
  <summary>What abjective of using ol, ul and dl for list or groups of links?</summary>

The objective of this technique is to create list of related items using list elements appropriate for their purpose. The ol element is used when the list is ordered and the ul element is used when the list is unordered. Description lists dl are used to group name-value pairs of inromation, for example: terms and definitions or questions and answers. Although the use of this markup can make lists more readable, not all lists need markup. For instance, sentance, sentences that contain comma-separated lists may not need list markup.

**Procedure:**

1. Check that content that has the visual appearance of a list is marked as an unordered list.
2. Check that content that has the visual appearance of a numbered list is marked as an ordered list.
3. Check that content is marked as a description list when groups of name-value pairs, for example: terms and definitions or questions and answers, are presented in the form of a list.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H48)

</details>

<details>
  <summary>What abjective of using semantic markup to mark emphasized or special text?</summary>

The objective of this technique is to demonstrate how semantic markup can be used to mark emphasised or special text so that it can be programmatically determined. Using semantic markup to mark emphasized or special text also provides structrue to the document. User agents can then make the structure perceivable to the user, for example using a different visual presentation for different types of structures or by using a different voice or pitch in an auditory presentation.

**Procedure:**

1. Examine the content for information that is conveyed through variations in presentation of text.
2. Check that appropriate semantic markup have been used to mark the text that conveys information through variations in text.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H49)

</details>

<details>
  <summary>What abjective of using table markup to present tabular infroamtion?</summary>

The objective of this technique is to present tabular infroamtion in a way that preserves relationships within the infroamtion even when users cannot see the table or the presentation format is changed. Inforamtion is considered tabular when logical relationships among text, numbers, images, or other data exist in two dimensions. These relationships are represented in columns and rows, and the columns and rows must be recognizable in order for the logical relationships to be perceived.

**Procedure:**

1. Check for the presence of tabular information.
2. For each occurrence of tabular inforamtion: check that table markup with at least the elements table, tr, th, and td is used.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H51)

</details>

<details>
  <summary>What abjective of using the body of the object element?</summary>

The objective of this technique is to provide a text alternative for content rendered using the object element. The body of the object element can be used to provide a complete text alternative for the object, or may contain additional non-text content with text alternatives.

**Procedure:**

1. Check that the body of each object element contains a text alternative for the object.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H53)

</details>

<details>
  <summary>What abjective of using the dfn element to identify the defining instance of a word?</summary>

The objective of this technique is to use the dfn to mark the use of a word or phrase where it is defined. The dfn element is used to indicate the defining instance of the enclossed term. In other words, it marks the occurrence of the term where the term is defined. Note that it encloses the term, not the difinition. This technique would be used in combination with Using inline definitions to provide the definition.

**Procedure:**

1. Identify all words that are defined inline in the text, that is where the definition occurs in a sentence near an occurrence of the word.
2. Check that each word that is defined inline is contained in a dfn element.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H54)

</details>

<details>
  <summary>What abjective of using the dir attribute on an inline element to resolve problems with nested directional runs?</summary>

The objective of this technique is to identify changes in the text direction of text that includes nested directional runs by providing the dir attribute on inline elements. A nested directional run is a run of text that includes mixed directional text, for example, a paragraph in English containing a quoted Hebrew sentence which in turn includes an English phrase. Use of the dir attribute on an enclosing span or other inline element may be necessary because the Unicode bidrectional algorithm can produce undesirable results when mixed directional text contains spaces or punctuation. The concepts used in this technique are described in What you need to know about the bidi algorithm and inline markup.

**Procedure:**

1. Examine the text direction of text in the document.
2. If the text direction is right-to-left, check that for the ancestor element that has a dir attribute, the attribute has the value rtl.
3. If the text direction is left-to-right, check that there is no ancestor element with a dir attribute, or that for the ancestor element that has a dir attribute, the attribute has the value ltr.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H56)

</details>

<details>
  <summary>What abjective of using the language attribute on the HTML element?</summary>

The objective of this technique is to identify the default language of a document by providing the lang attribute on the html element.

**Procedure:**

1. Check that the html element has a lang attribute.
2. Check that the value of the lang attribute conforms to tags for identifying languages or its successor and reflects the primary language used by the Web page.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H57)

</details>

<details>
  <summary>What abjective of using language attributes to identify changes in the human language?</summary>

The objective of this technique is to clearly identify any changes in language on a page by using the lang attribute.

**Procedure:**

For each element in the document:

1. Check that the human language of the content of the lement is the same as the inherited language for the element.

For each lang attribute in the document:

1. Check that the value of the lang attribute.
2. Check that the language code matches the language of the content it applies to.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H58)

</details>

<details>
  <summary>What abjective of using the ruby element?</summary>

The objective of this technique is to use ruby annotation to provide information about the pronunciation and meaning of a run of text where meaning is determined by pronunciation.

**Procedure:**

1. Check that a rt element contains pronunication infromation for each run of text defined by the rb element.
2. If simple Ruby markup is used, check that the rp element is present to indicate to user agents that do not support Ruby annotations that the text in the rt element provides the pronunciation information.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H62)

</details>

<details>
  <summary>What abjective of using the scope attribute to associate header cells with data cells in data tables?</summary>

The objective of this technique is to associate header cells with data cells in complex tables using the scope attribute. The scope attribute may be used to clarify the scope of any cell used as a header. The scope identifies whether the cell is a header for a row, column, or group of rows or comumns. The values row, col, rowgroup, and colgroup identify these possible scopes, respectively.

**Procedure:**

1. Check that all th elements have a scope attribute.
2. Check that all scope attributes have the value row, col, rowgroup, or colgroup.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H63)

</details>

<details>
  <summary>What abjective of using the title attribute of the iframe lement?</summary>

The objective of this technique is to demonstrate the use of the title attribute of the iframe element to describe its contents. This provides a label for the iframe so users can determine which frame to enter and explore in details. It does not label the content inside the iframe.

**Procedure:**

1. Check each iframe element in the HTML source code for the presence of a title attribute.
2. Check that the title attribute contains text that describes the iframe's content.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H64)

</details>

<details>
  <summary>What abjective of using the title attribute to identify form controls when the label element cannot be used?</summary>

The objective of this technique is to use the title attribute to provide an accessible name for form controls when the visual design does not include text on the screen that can be associated with the control as a label. User agents, including assistive technology, can speak the title attribute.

**Procedure:**

1. Check that the control has a title attribute.
2. Check that the purpose of the form control is clear to users who can see the control.
3. Check that the title attribute identifies the purpose of the control and that it matches the apparent visual purpose.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H65)

</details>

<details>
  <summary>What abjective of using null alt text and no title attribute on img elements for images that assistive technology should ignore?</summary>

The purpose of this technique is to show how images can be marked so that they can be ignored by assistive technology.

**Procedure:**

1. Check that title attribute is either absent or empty.
2. Check that alt attribute is present and empty.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H67)

</details>

<details>
  <summary>What abjective of providing heading elements at the beginning of each section of content?</summary>

The objective of this technique is to use section headings to convey the structure of the content. Heading markup can be used:

- to indicate start of main content;
- to mark up section headings within the main content area;
- to demarcate different navigational sections like top or main navigation, left or secondary navigation and footer navigation;
- to mark up images of text that are used as headings;
- to allow users the ability to navigate a page by sections or skip repeated blocks of information.

**Procedure:**

1. Check that the content is divided into separate sections.
2. Check that each section on the page starts with a headings.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H69)

</details>

<details>
  <summary>What abjective of providing a description for groups of from controls using fieldset and legent elements?</summary>

The objective of this technique is to provide a semantic grouping for related form controls. This allows users to understand the relationship of the controls and interact with the form more quickly and effectively.

**Procedure:**

1. Check that the group of logically related input or select elements are contained within fieldset elements.
2. Check that each fieldset has a legend element that is the first child in the fieldset and includes a description for that group.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H71)

</details>

<details>
  <summary>What abjective of using meta refresh to create an instant client-side redirect?</summary>

The objective of this technique is to enable redirects on the client side without confusing the user. Redirects are preferebly implemented on the server side, but authours do not always have control over server-side technologies.

**Procedure:**

Find all meta elements in the document that contain the http-equiv attribute with value refresh, check that:

1. The content attribute has a number with a value of 0.
2. The number is followed by; URL=anyURL (where anyURL stands for the URI that should replace the current page).

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H76)

</details>

<details>
  <summary>What abjective of identifying the purpose of a link using link text combined with its enclosing list item?</summary>

The objective of this technique is to identify the purpose of a link from the link and its list item context. The list imte enclosing the link provides context for an otherwise unclear link when the list item is the nearest enclosing block-level ancestor element. The description lets a user distinguish this link from links in the Web page that lead to other destinations and helps the user determine whether to follow the link. Note that simply providing the URI of the destination is generally not sufficiently descriptive.

**Procedure:**

1. Check that the link is part of a list item.
2. Check that text of the link combined with the text of its enclosing list item describes the purpose of the link.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H77)

</details>

<details>
  <summary>What abjective of identifying the purpose of a link using link text combined with its enclosing paragraph?</summary>

The objective of this technique is to identify the purpose of a link from the link and its paragraph context. The paragraph enclosing the link provides context for an otherwise unclear link when the paragraph is the nearest enclosing block-level ancestor element. The description lets a user distinguish this link from links in the Web page that lead to other destinations and helps the user determine whetehr to follow the link. Note that simply providing the URI of the destination is generally not sufficiently descriptive.

**Procedure:**

1. Check that the link is part of a paragraph.
2. Check that text of the link combined with the text of its enclosing paragraph describes the purpose of the link.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H78)

</details>

<details>
  <summary>What abjective of identifying the purpose of a link using link in a data table using the link text combined with its enclosing table cell and associated table header cells?</summary>

The objective of this technique is to identify the purpose of a link from the link in its data table context. This context is the table cell enclosing the link and the cell's associated table header cells. The data table context provides the purpose for an otherwise unclear link when the table cell is the nearest enclosing block-level ancestor element. IT lets a user distinguish this link from other links in the Web page that lead to other desinations and helps the user determine whether to follow the link. Note that simply providing the URI of the destination is not sufficiently descriptive for people with disabilities especially those with cognitive disabilities.

**Procedure:**

1. Check that the link is in a talbe cell.
2. Check that text of the link combined with the text of the associated table header cells describes the purpose of the link.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H79)

</details>

<details>
  <summary>What abjective of identifying the purpose of a link using link text combined with the preceding heading element?</summary>

The objective of this technique is to identify the purpose of a from the context provided by its heading context. The preceding heading provides context for an otherwise unclear link. The description lets a user distinguish this link from links in the Web page that lead to other destinations and helps the user determine whether to follow the link.

**Procedure:**

1. Find the heading element that precedes the link.
2. Check that the text of the link combined with the text of that heading describes the purpose of the link.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H80)

</details>

<details>
  <summary>What abjective of identifying the purpose of a link in a nested list using link text combined with the parent list item under which the list is nested?</summary>

The objective of this technique is to describe the purpose of a link in a nested list from the context provided by the list item under which the list is nested. This list item provides context for an otherwise unclear link. The description lets a user distinguish this link fro mlinks in the Web page that lead to other destinations and helps the user determine whether to follow the link.

**Procedure:**

1. Find the link's parent ul or ol element.
2. Check that this list element (ul, ol) is a descendant of an li element.
3. Check that the text of the link combined with the text of that parent li element describes the purpose of the link.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H81)

</details>

<details>
  <summary>What abjective of using the target attribute to open a new window on user request and indicating this in link text?</summary>

The objective of this technique is to avoid confusion that may be caused by the appearance of new windows that were not requested by the user. Suddenly opening new windows can disorient users or be missed completely by some. In HTML, the target attribute can be used to open a new window.

**Procedure:**

1. Activate each link in the document to check if it opens a new window.
2. For each link that opens a new window, check that it uses the target attribute.
3. Check that the link text contains information indicating that the link will opwn in a new window.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H83)

</details>

<details>
  <summary>What abjective of using a button with a select element to perform an action?</summary>

The objective of this technique is to allow the user to control when an action is performed, rather than having the action occur as a side effect of choosing a value for the select element. The user may inspect the different values of the select element, or may accidentally choose the wrong value, without causing the action to occur. When the user is satisfied with their choice, they select the button to perform the action.

**Procedure:**

1. Check that focus (including keyboard focus) on an option in the select element does not result in any actions.
2. Check that selecting the button performs the action associated with the current select value.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H84)

</details>

<details>
  <summary>What abjective of using optgroup to group option elements inside a select?</summary>

The objective of this technique is to group items in a selection list. A selection list is a set of allowd values for a form control such as a multi-select list or a combo box. Often selection list have groups of related options. Those groups should be semantically identified, rather than being delimiter with "dummy" list entries, for example: an option element containing only a series of dashes to create a horizontal line. Semantically identifying groups of options helps to visually break up long list so that users can more easily locate what they are interested in.

**Procedure:**

1. Check the set of options within a selection list to see if there are groups of related options.
2. If there are groups of related options, they should be grouped with optgroup.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/html/H85)

</details>
