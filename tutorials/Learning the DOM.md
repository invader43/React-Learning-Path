## Document Object Model
The Document Object Model (DOM) is a programming interface for web documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects; that way, programming languages can interact with the page.

### How to access it ?
```js
const paragraphs = document.querySelectorAll("p");
// paragraphs[0] is the first <p> element
// paragraphs[1] is the second <p> element, etc.
alert(paragraphs[0].nodeName);
```
The ```document``` object represents the document itself , in our case its the HTML document. The DOM is not part of the JavaScript language, but is instead a Web API used to build websites. JavaScript can also be used in other contexts. For example, Node.js runs JavaScript programs on a computer, but provides a different set of APIs, and the DOM API is not a core part of the Node.js runtime.

Another simple example using inline JavaScript :
```html
<html lang="en">
  <head>
    <script>
      // run this function when the document is loaded
      window.onload = () => {
        // create a couple of elements in an otherwise empty HTML page
        const heading = document.createElement("h1");
        const headingText = document.createTextNode("Big Head!");
        heading.appendChild(headingText);
        document.body.appendChild(heading);
      };
    </script>
  </head>
  <body></body>
</html>

```
### List of most used HTML tags
- ```<!DOCTYPE html>```: Declares the HTML version.
- <```html>```: Wraps the entire HTML document.
- ``` <head>```: Contains metadata like title, character set, styles, and scripts.
- ```<title>```: Sets the document title.
- ```<body>```: Contains the main content of the HTML document.
- ```<h1>``` to ```<h6>```: Define headings, where ```<h1>``` is the largest and ```<h6>``` is the smallest.
- ```<p>```: Represents paragraphs of text.
- ```<a>```: Creates hyperlinks, linking to another document or resource.
- ```<img>```: Embeds images.
- ```<ul>``` and ```<ol>```: Define unordered and ordered lists.
- ```<li>```: Represents list items within ```<ul>``` or ```<ol>```.
- ```<div>```: Groups content for styling or layout purposes.
- ```<span>```: Applies styles to inline elements.
- ```<br>```: Inserts a line break within text.
- ```<hr>```: Represents a horizontal rule or line.
- ```<strong>``` and ```<em>```: Emphasise text with strong and emphasised importance, respectively.
- ```<input>```: Creates input fields for forms.
- ```<form>```: Wraps form elements for user input.
- ```<table>```, ```<tr>```, ```<td>```, ```<th>```: Constructs tables, rows, and cells for tabular data.
- ```<iframe>```: Embeds external content, like a webpage or video, within the current document.
