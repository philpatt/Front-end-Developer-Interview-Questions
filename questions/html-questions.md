# HTML Questions:

* **What does a `doctype` do?**

*Required for legacy reasons. doctype ensures that the browser makes a best-effort attempt at following the relevant specifications. 
Think seatbelt analogy - You don’t know if you will need it*.

* **How do you serve a page with content in multiple languages?**

*Use the ‘lang’ attribute to set the language of the document*

* **What kind of things must you be wary of when design or developing for multilingual sites?**

*Pay attention to dialectal differences (i.e. US English and British English*

* **What are `data-` attributes good for?**

*Gives developer ability to store extra information that doesn’t have any visual representation*

* **Consider HTML5 as an open web platform. What are the building blocks of HTML5?**

*Semantics – allowing you to describe more precisiely what your content is*.

*Connectivity – allowing you to communicate with the server in new and innovative ways*.

*Offline and Storage – allowing webpages to store data on the client-side locally and operate offline more efficiently*.

*Multimedia – making video and audio first-class citizens in the Open Web*.

*2D/3D graphics and effects ¬– allowing a much more diverse range of presentation options*.

*Performance and integration – providing greater speed optimization and better usage of computer hardware*.

*Device access – allowing for the usage of various input and output devices*.

*Styling – letting authors write more sophisticated themes*.

* **Describe the difference between a `cookie`, `sessionStorage` and `localStorage`.**

*sessionStorage, localStorage, and Cookies all are used to store data on the client side. Each one has its own storage and expiration limit*.

*localStorage – stores data with no expiration date, and gets cleared only through Javascript, or clearing the Browser Cache / locally stored data*.

*sessionStorage – similar to localStorage but expires when the browser closes (not the tab)*.

*Cookie – stores data that has to be sent back to the server with subsequent requests. Its expiration varies bsed onteh type and the expiration duration can be set from either server-side or client-side (normally from server-side)*.

* **Describe the difference between `<script>`, `<script async>` and `<script defer>`.**

*`<script>` is default behavior of `<script>` element. Parsing of the HTML code pauses while the script is executing. For slow servers and heavy scripts this means that isplaying the webpage will be delayed*.

*`<script defer>` Delaying script executing until the HTML parser has finished. Apositive effect of this attribute is that the DOM will be available for your script - however not every browser supports defer - is the equivalent of jQuery.ready()*

*`<script async>` HTML parsing may continue and the script will be executed as asson as its ready. Recommended for scripts such as Google Analytics*

* Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions?

*CSS `<link>`s should be in between `<head></head>` to prevent Flash of Unstyled Content which gives the user something to look at while the rest of the page is being parsed*

*Since Javascript blocks rendering by default, and the DOM and CSSOM construction can be also be delayed, it usually best to keep scripts at the bottom of the page*

*Exceptions are if you grab the scripts asynchronously, or at least defer them to the end oof the page*

* What is progressive rendering?
*Progressive rendering of HTML is chunking the HTMl into separate bits and loading each chunk as its finished. Usually, the backend code loads the HTMl at once, but if you flush after finishing one part of the structre, it can be rendered immediately to the page*

* Why you would use a `srcset` attribute in an image tag? Explain the process the browser uses when evaluating the content of this attribute.

*`srcset` allows you to specify different kind of images for different screen-sizes/orientation/display-types. The usage is really simple, you just provide a lot of diffeent images separating them with a comma like this: `<img src="image.jpg" alt="image" srcset="<img> <descriptor>, ..., <img_n> <descriptor_n>">` Here is an example: `srcset="image.jpg 160w, image2.jpg 320w, image3.jpg 2x"`*

* Have you used different HTML templating languages before?

*I have experience using Embedded Javascript (EJS). This Templating language lets you generatl HTML markup with plain javascript. I typically use this with Node.js and React.js*

