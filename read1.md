# Massage for ASAC student 

Dears you are so lucky if you got chance to learn software at ASAC collage, I will not talk about the impressive environment but i will talk about what you going to learn here.

Today i will talk about Git and GitHub but what the different between them? 

***The photos below tell us bout the different between them***

![photo](https://blog.devmountain.com/hs-fs/hubfs/Imported_Blog_Media/Gitvs_Github-1a-1.jpg?width=600&name=Gitvs_Github-1a-1.jpg)

But please don't confuse we will go through some detials in the Github now.

Before stat learn on the GitHub you have to down load and installation many of software like GitHub, ubuntu, visual studio, terminal command and connect between them
![ubunto](https://machiine.com/wp-content/uploads/2013/02/github-plus-ubuntu.jpg)

#### After that you need to follow steps to start coding (New steps if you use another software): 
1. Create a repository
   Head over to GitHub and create a new public repository named username.github.io, where username is your username (or organization name) on GitHub.

2. Clone the repository 
```
  $ git clone https://github.com/username/username.github.io
```
3. Hello World
```
   $ cd username.github.io

   echo "Hello World" > index.html
```

#### What the teacher expect from you after learn markdown 

1. Markdown format makes styled collaborative editing easy
2. Markdown differs from traditional formatting approaches
3. use Markdown to format text
4. leverage GitHub’s automatic Markdown rendering
5. apply GitHub’s unique Markdown extensions

but befor that you should to know what is the markdown 

**Markdown**:is a way to style text on the web. You control the display of the document; formatting words as bold or italic, adding images, and creating lists are just a few of the things we can do with Markdown.

**Where you can use Markdown :**
+ Gists
+ Comments in Issues and Pull Requests
+ Files with the .md or .markdown extension

**Here some examples**

######1.Text 

``
It's very easy to make some words **bold** and other words *italic* with Markdown. You can even [link to Google!](http://google.com)
``
**Out put on the repo**
It's very easy to make some words **bold** and other words *italic* with Markdown. You can even [link to Google!](http://google.com)

######1.Syntax *Heading*

```
# This is an <h1> tag
## This is an <h2> tag
###### This is an <h6> tag
```
**Out put on the repo**
# This is an <h1> tag
## This is an <h2> tag
###### This is an <h6> tag

**Example of GitHub flavor Markdown**

###### Syntax highlighting
Here’s an example of how you can use syntax highlighting with GitHub Flavored Markdown

```javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```
###### Tasklist

```
- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item
If you include a task list in the first comment of an Issue, you will get a handy progress indicator in your issue list. It also works in Pull Requests!
```

Output
- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item
If you include a task list in the first comment of an Issue, you will get a handy progress indicator in your issue list. It also works in Pull Requests!

###### Tables
You can create tables by assembling a list of words and dividing them with hyphens - (for the first row), and then separating each column with a pipe |:
```
First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column
```
Output
First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column

#### Emoji
you can add emoji by using special code from [Emoji Cheat Sheet] (https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README)