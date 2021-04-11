# HTML Text, CSS Introduction, and Basic JavaScript Instructions

![p](https://miro.medium.com/max/6300/1*l4xICbIIYlz1OTymWCoUTw.jpeg)

Topics:
1. HTML text
2. Introduction CSS
3. Basic JavaScript instruction
4. Decisions and loops 

I think from last repo you had understand how to creat simple webpage by using html and js and here we will go through deeply to introduce the relations between three brothers html css and js 

lets tie belts and start...

## HTML text
At the begining we will talk about html text 

In this section we focus on how to add markup to the text that appears on your pages. You will learn about:
**Structural markup:** the elements that you can use to
describe both headings and paragraphs
**Semantic markup:** which provides extra information; such as where emphasis is placed in a sentence, that something you have written is a quotation (and who said it), the meaning of acronyms, and so on

we can summarize tags that used to edit of the text in one paragraph. 
then i will give you comprehensive example to make you fully under stand.

![htmltage](http://static1.squarespace.com/static/58dd0c8cd482e901dc8ea61e/59cc09829f8dce4098e5c426/5ac405760e2e72d53c1499da/1522968217225/HTML-Tags-Book-Description-Square-Chart.png?format=1500w)

```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>

<body>
    <h1>My name is Bara'a</h1>
    <h2>My name is Bara'a</h2>
    <h3>My name is Bara'a</h3>
    <h4>My name is Bara'a</h4>
    <h5>My name is Bara'a</h5>
    <h6>My name is Bara'a</h6>
    <!-- in this pargrapg i will include all text tages edits -->
    <p>Lorem <b> dolor</b> sit amet <em>adipisicing elit.</em>  Reiciendis <i>deleniti odio aspernatur</i>, provident vitae
        omnis, numquam at corrupti voluptatibus, blanditiis dolores suscipit aliquid iure dolorem veniam saepe nobis ab!
        Pariatur <strong> quae neque fugiat iure odit</strong> expedita quam, <sub> molestias</sub> earum, ipsum optio, fugit animi
        quidem ea dolores cupiditate vel.</p>
        <br>
        <hr>
    <p>Lorem ipsum dolor sit amet <ul>consectetur, adipisicing elit.</ul> Dolores voluptates beatae id porro, tempora maxime a,
        deleniti fuga fugit quisquam ad rerum ea <strick>reiciendis animi delectus nobis sequi? Nemo,</strick> debitis.</p>
</body>

</html>
```

![pic6](./img/pic6.png)

Also we have many of tags that usedin html like `<del>` and `<adress>` but they are doesn't used daily in your work 

##### Summary 

* HTML elements are used to describe the structure of the page (e.g. headings, subheadings, paragraphs).
* They also provide semantic information (e.g. where emphasis should be placed, the definition of any acronyms used, when given text is a quotation).


# Introduction CSS

If you like designs and shapes you will have fun here becuase we will talk about fun part in webpages developing.
In this section, we will look at how to make your web pages more attractive, controlling the design of them using CSS.
CSS allows you to create rules that specify how the content of an element should appear. For example, you can specify that the background of the page is cream, all paragraphs should appear in gray using the Arial typeface, or that all level one headings should be in a blue, italic, Times typeface.

CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration.

![css](https://hackernoon.com/drafts/2z4a3yh4.png)

* Selectors indicate which element the rule applies to. The same rule can apply to more than one element if you separate the element names with commas.
* Declarations indicate how the elements referred to in the selector should be styled. Declarations are split into two parts (a property and a value), and are separated by a colon.

If you need to apply your design you have three ways that you can refer to them in the last repo:

1. inline
it will be inline leterly

```
<h1 style="color:blue;">A Blue Heading</h1>
```

2. internal 
by using style tage in head in html file 

```
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

3. external
it is important to link html file with css file by use link tag in head of html as below 

```
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```


```
body {
  background-color: lightblue;
}

h1 {
  color: navy;
  margin-left: 20px;
}
```

There are many different types of CSS selector that allow you to target rules to specific elements in an HTML document. The table on the opposite page introduces the most commonly used CSS selectors.

CSS selectors are case sensitive, so they must match element  names and attribute values exactly.

![selector](./img/p7.png)

##### Summary 

* CSS treats each HTML element as if it appears inside its own box and uses rules to indicate how that element should look.
* Rules are made up of selectors (that specify the elements the rule applies to) and declarations (that indicate what these elements should look like).
* Different types of selectors allow you to target your rules at different elements.
* Declarations are made up of two parts: the properties of the element that you want to change, and the values of those properties. For example, the font-family property sets the choice of font, and the value arial specifies Arial as the preferred typeface.
* CSS rules usually appear in a separate document, although they may appear within an HTML page.

## Basic JavaScript instruction

In this section, you will start learning to read and write JavaScript. You wil l also learn how to give a web browser instructions you want it to follow.

JAVASCRIPT IS CASE SENSITIVE
JavaScript is case sensitive so hourNow means something different to HourNow or HOURNOW.

A script will have to temporarily store the bits of information it needs to do its job. It can store this data in variables.

```
var baRa=25;
/* we can write comment like this also in js*/
//or like this
```

What abut data type of JS, data type will shown below in the table.

![datatype](https://www.miltonmarketing.com/wp-content/uploads/2018/04/Introduction_to_JavaScript-_Review_Types_and_OperatorsJavascript3.png)

![datatype2](https://www.wisdomjobs.com/tutorials/data-types.jpg)

* Array:JavaScript arrays are used to store multiple values in a single variable.

What is an Array?
An array is a special variable, which can hold more than one value at a time.

```
var cars = ["Saab", "Volvo", "BMW"];
document.getElementById("demo").innerHTML = cars;
```


##### Summary

* A script is made up of a series of statements. Each statement is like a step in a recipe.
* Scripts contain very precise instructions. For example, you might specify that a value must be remembered before creating a calculation using that value.
* Variables are used to temporarily store pieces of information used in the script.
* Arrays are special types of variables that store more than one piece of related information.
* JavaScript distinguishes between numbers (0 -9), strings (text), and Boolean values (true or false).
* Expressions evaluate into a single value.
* Expressions rely on operators to calculate a value.

## Decisions and loops

Decision Making in programming is similar to decision making in real life.
A programming language uses control statements to control the flow of execution of the program based on certain conditions. JavaScript’s conditional statements are:
1. if
2. if-else
3. if else if
4. switch

**if statement**
if statement is the most simple decision making statement.
It is used to decide whether a certain statement or block of statements will be executed or not.
If a certain condition is true then a block of statement is executed otherwise not.

Syntax
if ( condition )

```
{
   // block of code to be executed
}
```

You can omit the braces if there is only single statement in block.

***if else statement***
The if-else statement has two parts if block and else block.
If the condition is true then if block (true block) will get executed and if the condition is false then else block (false block) will get executed.

Syntax

```
if ( condition )  
{
    // block of code to be executed when condition is true
} 
else 
{
    // block of code to be executed when condition is false
}
```  


**if…else...if statement**
The if…else…if statement statement is an advanced form of if…else that allows JavaScript to make a correct decision out of several conditions.
All the if conditions will be checked one by one. If any condition is true out of given then that block will get executed and other blocks are skipped.

Syntax

```
if ( condition 1 )  
{
    // block of code to be executed when condition 1 is true
} 
else if ( condition 2 )  
{
    // block of code to be executed when condition 2 is true
} 
else if ( condition 3 )  
{
    // block of code to be executed when condition 2 is true
}
else
{
   // block of code to be executed if no condition matches
}
```

**switch statement**
The objective of a switch statement is to give an expression to evaluate and several different statements to execute based on the value of the expression.
The interpreter checks each case against the value of the expression until a match is found. If nothing matches, a default condition will be used.

Syntax

```
switch (expression) 
{
   case c1: statement(s)
            break;
   
   case c2: statement(s)
            break;
   ...
   
   case cn: statement(s)
            break;
   
   default: statement(s)
}
```

***Looping Statements***

Looping in programming languages facilitates the execution of a set of instructions/functions repeatedly while some condition evaluates to true.
For example, suppose we want to print “Hello World” 10 times this is possible with the help of loops.
There are mainly two types of loops:

1. Entry Controlled loops: In this type of loops the test condition is tested before entering the loop body. For Loop and While Loop are entry controlled loops.
2. Exit Controlled Loops: In this type of loops the test condition is tested or evaluated at the end of loop body. Therefore, the loop body will execute atleast once, irrespective of whether the test condition is true or false. do-while loop is exit controlled loop.
Following are the types of loops in JavaScript:

1. while loop
2. do-while loop
3. for loop
4. for…in loop


1. while loop

A while loop is a entry-controlled loop that allows code to be executed repeatedly if the condition is true.
When the condition becomes false, the loop terminates which marks the end of its life cycle.
The while loop executes ZERO or MORE times.

Syntax

```
while (condition)
{
   // Statements to be executed
}
```


2. do-while loop

A do-while loop is a exit-controlled loop that allows code to be executed first and after that checks for condition and depending on that it executed repeatedly.
When the condition becomes false, the loop terminates which marks the end of its life cycle.
The do-while loop executes ONE or MORE times.

Syntax

```
do
{
    // Statements to be executed
}  while (condition);
```


3. for loop

A for loop is a entry-controlled loop that allows code to be executed repeatedly.
It provides a concise way of writing the loop structure.
Unlike a while loop, a for statement consumes the initialization, condition and increment/decrement in one line thereby providing a shorter, easy to debug structure of looping.
The for loop executes ZERO or MORE times

Syntax

```
for (initialization; condition; increment/decrement)
{
    // Statements to be executed
}
```

4. for-in loop

JavaScript also includes another version of for loop also known as the for..in loops.
The for..in loop provides a simpler way to iterate through the properties of an object.
This loop is seen to be very useful while working with objects.
In each iteration, one of the properties of Object is assigned to the variable named variableName and this loop continues until all of the properties of the Object are processed.

Syntax

```
for (variableName in Object)
{
    // Statements to be executed
}
SAMPLE PROGRAMS
Develop a JS program to display numbers from 1 to 10.
<html>
    <head>
        <title>Display Numbers from 1 to 10</title>
    </head>
    <body>
        <h3>Numbers from 1 to 10 are</h3>
        <script type="text/javascript">
            var a = 1; 
  
            while (a <= 10) 
            { 
                document.write(a + "<br />"); 
                a++; 
            }
        </script>
    </body>
</html>
```