# Wire Fram, HTML & CSS Intro

![Photo](https://miro.medium.com/max/675/1*dqLV7KjUtg57JPBCilqxSQ.jpeg)

## Wire Fram = Structure 
   structure is very important in helping readers to understand the messages you are trying to convey and to navigate around the document.

At the beginning you need to draw your web structure by using paper or online application to find initial design or structure of your website, and it will called **wirefame**

Scratch| miro.com
---------|----------
![1](https://careerfoundry.com/en/blog/uploads/Wiregraming_PillarPage.jpg)|![2](https://i.ytimg.com/vi/zQ3Cn3EQz3k/maxresdefault.jpg)

## HTML describeS the Structure

In the figure below you can find the html structure of the web bages

Html 5 head| Html 5 body
-------|----------
![photo](https://www.oreilly.com/library/view/learning-web-design/9781449337513/httpatomoreillycomsourceoreillyimages2257981.png)|![p](https://assets.hongkiat.com/uploads/html-5-semantics/document-outline-example.jpg)

## HTML tages that should all programmer deal with them 

![tage](https://mason.gmu.edu/~kshiffl4/375/HTML_Tags.jpg)

## But what the different between HTML&CSS

![k](https://miro.medium.com/max/2400/1*eGqxygcyUDxBo0lgYdvssQ.png)


HTML |css
----|-----
HTML stands for Hyper Text Markup Language.it is a scripting language used for making websites.it describes the structure of a webpage.Html consists of Elements,Attributes and Tags.|CSS is a Cascading Style Sheet.it describes how HTML elements are to be displayed on screen,through this we can change the presentation and not the structure.Declaration should be in property :value pair.Like HTML there are lots of properties in Css too.
![m](https://miro.medium.com/max/554/1*4pO33ZUyJ0JBia-W4-P8XQ.png)|![j](https://miro.medium.com/max/569/1*VjE5xYOMx_8x0Z7td2JvaA.gif)

## How to link CSS with HTML?

1. **Inline:** The Inline style is specific to the tag itself. The inline style uses the HTML “style” attribute to style a specific tag. This is not recommended, as every CSS change has to be made in every tag that has the inline style applied to it. The Inline style is good for one an individual CSS change that you do not use repeatedly through the site.

**Example** 
```
<body>
<p style="color:red;margin-left:30px;">This is paragraph</p>
</body>
```
2. **Internal:** An internal stylesheet holds the CSS code for the webpage in the head section of the particular file. This makes it easy to apply styles like classes or id’s in order to reuse the code.

**Example** 
```
<head> 
<style type="text/css">  
h1 {color:blue;}  
h2 {color:red;}  
p {color:green;} 
</style>  
</head>
```
3. **External:** The External Stylesheet is a .css file that you link your website to. This makes it so that what ever you change in the .css sheet, will effect every page in your website. This prevents you from having to make many code changes in each page. This is for “global” site changes.

**Example** 
```
<head>
<link rel="stylesheet" type="text/css" href="style.css" />
</head>
```