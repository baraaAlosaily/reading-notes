# Problem Domain, Objects, and the DOM

JavaScipt DOM Tree
![dom](https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2019/08/JavaScript-Dom-Tree.png)

**JavaScript Document Object Model (DOM)**
A Document Object Model is a programming interface for HTML (HyperText Markup Language) and XML (eXtensible Markup Language) documents. It provides a data representation comprising all the objects, depicting the structure and content of the document on the web. Every webpage has its own DOM that represents the page so that programs can alter its structure, look, and content.

In simpler terms, when a browser loads a webpage, it creates a model of that page. This model is the DOM tree and is filed in the browser’s memory. It provides functionality globally to the document, including how to obtain the page details and create new elements in the document. Remember, DOM is neither a part of HTML nor JavaScript; it’s a separate set of rules. All the major browser makers implement it and it covers two primary sections:

1. Creation of the DOM tree
2. Manipulation of the DOM tree

We will cover both these areas in this reading-notes so you will understand how JavaScript actually works with the DOM. For now, let’s see what a DOM tree looks like and its different components with the help of a program.

**Program**

```
<html>
  <head>
    <title>DOM Model</title>
  </head>
  <body>
    <h1>DataFlair’s Tutorial</h1>
    <p>DOM Tree</p>
    <p id = "text">This is a text element in the DOM tree.</p>
  </body>
</html>
```

Every element, attribute, and text content in the HTML creates its own DOM node in the tree. A DOM tree consists of four main types of nodes:

- Document node:
  This is added at the top of the tree and represents the entire page in the browser. As stated above, it is the starting point in the DOM tree; you need to navigate via the document node to access any other node in your DOM tree.

- Element nodes:
  All the HTML elements like heading tags (`<h1>` to `<h6>`) and paragraph tags (`<p>`) in the page create an element node in the tree. You use these nodes to gain access to the elements’ attribute and text nodes.

- Attribute nodes:
  When the opening tags in the HTML document contain attributes, the tree represents them as attribute nodes. These are not the children of the element nodes but a part of them.

- Text nodes:
  Once you have access to the element node, you can reach the text content within that element, stored inside the text nodes of the DOM tree. These nodes cannot have child nodes. Thus, a text node always creates a new branch in the DOM tree, and no further branches come out of it.

### Working with the DOM Tree in JavaScript DOM

To access and modify the DOM tree, you need to follow two steps:

Locate the node representing the element you want.
Works with the node’s content, child elements, and attributes.

![w](https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2019/08/Js-Dom-Tree.png)

Accessing the Elements
DOM Queries are the methods that find elements in the DOM tree. They may return one element or a collection of elements in a NodeList. You can select any element you desire from the NodeList with the help of an index number (starting with 0).

The code mentioned below is the HTML and CSS code, common to all the examples. All you would need to do is add the JavaScript code you want to execute.

Code:

```
<html>
  <head>
    <!-- CSS styling -->
    <style type="text/css">
      #page{
        max-width: 400px;
            margin: 20px auto 20px auto;
            border: 3px solid aqua;
      }
      h1, h2, ul{
        padding: auto;
      }
      p{
        text-align: center;
        font-size: large;
        font-weight: bold;
      }
    </style>
  </head>
  <body>
    <div id="page">
      <h1 id="header">TO DO LIST</h1>
      <ul>
        <h2>DataFlair’s JavaScript Tutorial</h2><DataFlair’s>
        <li id="one" class="mandatory">Learning the concepts</li>
        <li id="two" class="mandatory">Practising the codes</li>
        <li id="three">Taking quizzes</li>
        <li id="four">Solving Interview Questions</li>
      </ul>
      <!-- JavaScript code -->
    </div>
  </body>
</html>
```

**Summary**
Here we come to the end of our article on JavaScript DOM. In this article, we discussed every aspect of the Document Object Model (DOM). We understood how we can access the elements of a DOM tree and how to update them. In the end, we also learned how to add and/or remove an HTML element.
