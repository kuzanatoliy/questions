# HTML

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

  * Firstly, JavaScript code can be between open/close scripts tags.

  `<script>...your code</script>`

  * Secondly, the script tag can inject an external script. For it, need to add an src attribute with link to the external script.

  `<script src=’...’ />`

  **Note:** cannot mix these two ways. One script tag cannot have external and internal scripts at the same time. In this case, the browser runs the only external script.

  Also, the best place for script injection is the last part of the HTML document before close body tag because when a browser starts work with a script tag, it stops other processes before the script is loaded and run. Besides, there are async and defer attributes for async loading.

</details>

<details>
  <summary>Can a browser use async scripts loading? How? There is a difference between async and defer?</summary>
  
  The async loading of external scripts is allowed by async and defer attributes of a script tag. This functionality could be useful when to need to add additional functionality that not depend on others. For example, advertising banners. So, there are two ways to set async loading.
  
  * Firstly, to add an async attribute to a script tag. In this case, the script will be loaded async and run right after loading.
  
  * Secondly, to add a defer attribute to the tag. In this case, a browser run scripts after finish load all sources. Moreover, there will save the order of the loaded scripts.

  For example, try to imagen that we have five scripts like these:

  `<script class=’script1’ ...  />`
  `<script class=’script2’ deffer ...  />`
  `<script class=’script3’ deffer ...  />`
  `<script class=’script4’ async ...  />`
  `<script class=’script5’ ...  />`

  So, there is next order of the scripts runing: script1 -> script5 -> script4 -> script2 -> script3

</details>

<details>
  <summary>How does a browser render an HTML page?</summary>
  In progress ...
</details>

<details>
  <summary>What is new in the HTML5?</summary>
  In progress ...
</details>

<details>
  <summary>There is a difference between strong and b tags?</summary>
  In progress ...
</details>

<details>
  <summary>Why are semantic tags needed?</summary>
  In progress ...
</details>

<details>
  <summary>How can we join input and label?</summary>
  In progress ...
</details>

<details>
  <summary>What is the difference between vector and raster images?</summary>
  In progress ...
</details>

