jquery.json2html
=========

What is jquery.json2html?
------------------
jquery.json2html is a jquery plug-in that implements the HTML templating engine <a href='https://github.com/moappi/json2html'>json2html</a> for client side browers

Ok so what is json2html?
------------------
json2html is a javascript HTML templating engine which converts json object to html using json transforms.  Note that this jquery.json2html package includes the latest version of json2html.

For more information check out the <a href='https://github.com/moappi/json2html'>json2html</a> core library

Also implemented in node.js <a href='https://github.com/moappi/node-json2html'>node-json2html</a>


Why json2html?
--------------
Instead of writing HTML templates json2html relies on JSON transforms to convert a source JSON objects to html.  The benefit of using a JSON transform is that they are already readable by the browser and DO NOT require any compilation before use.   In addition, json2html allows the following

+	Short hand notation for mapping data objects to markup
+	Event binding to DOM objects (exclusively with jquery.json2html) 
+	Use of inline functions to allow for complex logic during transformation 
+	Dynamic building of transform objects

Example of a Transform?
--------------
```javascript
var transform = 
 {"<>":"li","id":"${id}","html":[
	{"<>":"span","html":"${name} ${year}"}
  ]};		
```
Will render into the following html

```html
<li id=1123>
	<span>Jack and Jill (2001)</span>
</li>	
```

Where is the project now?
--------------
json2html (and jquery.json2html) have been battle hardened and used in thousands of projects since it's original release in 2012.


How do I start?
--------------
Check out our website <a href='http://www.json2html.com'>www.json2html.com</a> for more information including detailed usage notes, downloadable examples and more!
