# HTML

### Links

[WebP](https://developers.google.com/speed/webp)

### Questions

<details>
  <summary>What is HTML?</summary>

HTML is the hypertext markup language. It is one of the XML types that allows describing document structure in a browser-friendly view.

</details>

<details>
  <summary>Why is a doctype tag needed? What will happen if there is no doctype in the HTML document?</summary>

Doctype allows understanding what type of the HTML standards browser should use for a document. Without this tag, a browser will work in compatibility mode. As a result, experimental features can be used that can break a document view.

</details>

<details>
  <summary>How can JavaScript be used on an HTML page? Where is the better place for injecting scripts to the page?</summary>

For working with JavaScript, HTML document has a script tag. There are two opportunities for injection scripts:

- Firstly, JavaScript code can be between open/close scripts tags.

`<script>...your code</script>`

- Secondly, the script tag can inject an external script. For it, need to add an src attribute with link to the external script.

`<script src=’...’ />`

**Note:** cannot mix these two ways. One script tag cannot have external and internal scripts at the same time. In this case, the browser runs the only external script.

Also, the best place for script injection is the last part of the HTML document before close body tag because when a browser starts work with a script tag, it stops other processes before the script is loaded and run. Besides, there are async and defer attributes for async loading.

</details>

<details>
  <summary>Can a browser use async scripts loading? How? There is a difference between async and defer?</summary>

The async loading of external scripts is allowed by async and defer attributes of a script tag. This functionality could be useful when to need to add additional functionality that not depend on others. For example, advertising banners. So, there are two ways to set async loading.

- Firstly, to add an async attribute to a script tag. In this case, the script will be loaded async and run right after loading.

- Secondly, to add a defer attribute to the tag. In this case, a browser run scripts after finish load all sources. Moreover, there will save the order of the loaded scripts.

For example, try to imagen that we have five scripts like these:

`<script class=’script1’ ... />`<br>
`<script class=’script2’ deffer ... />`<br>
`<script class=’script3’ deffer ... />`<br>
`<script class=’script4’ async ... />`<br>
`<script class=’script5’ ... />`

So, there is next order of the scripts runing: script1 -> script5 -> script4 -> script2 -> script3

</details>

<details>
  <summary>How does a browser render an HTML page?</summary>

Loading of a web page starts from a request for an HTML document. After that, a browser parse parts of the gotten documents and generate the document object model. When the browser finds a link to external sources as styles, images or scripts, it requests a new resource. Part of the requests could be blocking (It meant that browser stop other actions before those requests are loading). Next browser builds a CSS object model. After that, the browser generates a render tree where consulate styles for each element on the page. Next is a layout stage that defines elements positions on the web page. And finally, browser paint web page.

In details:

1. The Document Object Model is defined from tokens those were gotten from responses in HTML view and turn into nodes. They start from the start tag and end to end tag. Nodes content all necessary information about the HTML element and have a connection with render three through tokens. Note: Time of document processing depends on the count of nodes.
2. Download styles and build the CSS Object Model (CSSOM). It contents nodes with CSS styles of elements.
3. After that, the browser forms render tree from the DOM and the CSSOM. The render tree duplicates DOM without invisible elements as the head. Render tree's nodes contain the DOM element or text element and style.
4. Next one is the layout. For each render tree element calculate a position on document view.
5. Browser paint elements in the window.

_Repaint_ - happen when styles are changed, but proportions and position are not changed browser just repaint it.

_Reflow_ - happen when proportions and positions are changed. It could happen from the reasons:

- DOM manipulation (add, remove, change of nodes);
- Content changing;
- Calculation and changing of CSS properties;
- Adding, removing CSS layouts;
- Manipulation of class attributes;
- Resizing of browser proportions;
- Activation of pseudo-classes (for example, :hover).

</details>

<details>
  <summary>What is new in the HTML5?</summary>

- Canvas, tag for management of 2D graphic arts. Can be used for creating dynamic images and charts;
- Video and audio, tags add functionality for working with audio and video content without additional technologies;
- Context menu, opportunity adding context menus in your site;
- Semantic tags as a header, a footer, a main and etc., tags add better structure and have semantic meaning;
- New types for input tag as DateTime, Date, Week, URL, Email, etc., expand functionality for control elements;
- Syntaxis for settings of charset;
- Href attribute for links is necessary now;
- Async attribute for scripts.

</details>

<details>
  <summary>There is a difference between strong and b tags?</summary>

These tags have the same styles, but strong has a semantic meaning too. For example, readers can make attention to that text.

</details>

<details>
  <summary>Why are semantic tags needed?</summary>

There are a few reasons:

- Firstly, semantic tags allow implementing HTML pages with better structure;
- Secondly, these tags have meaning, that allows boots to made more effective working process.

</details>

<details>
  <summary>How can we join input and label?</summary>

There are two ways of joining input and label tags.
Firstly, an input tag can be pushed into a label tag.

`<label><input type=”text”><label>`

Secondly, a ‘for’ attribute of a label tag can content id of an input tag.

`<label for=”inputid”>Title</label>`<br>
`<input id=”inputid” type=”text” />`

</details>

<details>
  <summary>What is WebP image format?</summary>

WebP is a modern image format that provides superior lossless and lossy compression for images on the web. Using WebP, webmasters and web developers can create smaller, richer images that make the web faster.
[Support](https://caniuse.com/webp)

</details>
