# JavaScript Intro

## How JavaScript Makes Web pages More Interactive 
![js](https://mk0setscholarsn9sko6.kinstacdn.com/wp-content/uploads/2020/07/javascript.jpg)

***Javascript allow you to make web pae more interactive by accessing and modifying the content and markup used in the web pages while it is being viewed in the browser*** 

**1. ACCESS CONTENT**
     You can use JavaScript to select any element, attribute, or text from an
HTML page. For example:
- Select the text inside all of the `<hl> `elements on a page
- Select any elements that have a c 1 ass attribute with a value of note
- Find out what was entered into a text input whose id attribute has a value of ema i 1

**2. Modifying the content**
You can use JavaScript to add elements, attributes, and text to the page, or remove them. For example:
- Add a paragraph of text after the first `<hl>` element
- Change the value of c 1 ass attributes to trigger new CSS rules for those elements
- Change the size or position of an `<i mg> `element

**3. PROGRAM RULES**
You can specify a set of steps for the browser to follow (like a recipe), which allows it to access or change the content of a page. For example:
- A gallery script could check which image a user clicked on and display a larger version of that image.
- A mortgage calculator could collect values from a form, perform a ca lculation, and display repayments.
- An animation could check the dimensions of the browser window and move an image to the bottom of the viewable area (also known as the viewport).

**4. React ro event**

You can specify that a script should run when a specific event has occurred. For example, it could be run when:
- A button is pressed
- A link is clicked (or tapped) on
- A cursor hovers over an element
- Information is added to a form
- An interval of time has passed
- A web page has finished loading

### Data Types in JS

![jss](https://1.bp.blogspot.com/-EPrHJaCTGoU/X3MajXYktEI/AAAAAAAAB5E/qgkmTg0A0s0aRzvsmhmGpa3z2r9bQjIYwCLcBGAsYHQ/w400-h281/668dfc002312ab58e0d1cb15e0b98a5e.png)


### Same main tools of the java script

***1. JavaScript Syntaxis***

   JavaScript syntax is the set of rules, how JavaScript programs are constructed:
```
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Statements</h2>

<p>A <b>JavaScript program</b> is a list of <b>statements</b> to be executed by a computer.</p>

<p id="demo"></p>

<script>
var x, y, z;  // Statement 1
x = 5;        // Statement 2
y = 6;        // Statement 3
z = x + y;    // Statement 4

document.getElementById("demo").innerHTML =
"The value of z is " + z + ".";  
</script>

</body>
</html>
```

***2. JavaScript Operators***

Assign values to variables and add them together:

```
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Operators</h2>

<p>x = 5, y = 2, calculate z = x + y, and display z:</p>

<p id="demo"></p>

<script>
var x = 5;
var y = 2;
var z = x + y;
document.getElementById("demo").innerHTML = z;
</script>

</body>
</html>
```

***3. Function***

A JavaScript function is a block of code designed to perform a particular task.
A JavaScript function is executed when "something" invokes it (calls it).

```<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Functions</h2>

<p>This example calls a function which performs a calculation, and returns the result:</p>

<p id="demo"></p>

<script>
function myFunction(p1, p2) {
  return p1 * p2;
}
document.getElementById("demo").innerHTML = myFunction(4, 3);
</script>

</body>
</html>
```

***4. Conditional Statements***

Very often when you write code, you want to perform different actions for different decisions.
You can use conditional statements in your code to do this.
In JavaScript we have the following conditional statements:

- Use if to specify a block of code to be executed, if a specified condition is true
- Use else to specify a block of code to be executed, if the same condition is false
- Use else if to specify a new condition to test, if the first condition is false
- Use switch to specify many alternative blocks of code to be executed

```<!DOCTYPE html>
<html>
<body>

<p>Click the button to get a time-based greeting:</p>

<button onclick="myFunction()">Try it</button>

<p id="demo"></p>

<script>
function myFunction() {
  var greeting;
  var time = new Date().getHours();
  if (time < 10) {
    greeting = "Good morning";
  } else if (time < 20) {
    greeting = "Good day";
  } else {
    greeting = "Good evening";
  }
  document.getElementById("demo").innerHTML = greeting;
}
</script>

</body>
</html>
```

***5. Assignment Operators***

Assignment operators assign values to JavaScript variables.
![l](https://www.devopsschool.com/blog/wp-content/uploads/2020/08/assignment-operator-in-python.png)

***6. Window prompt() Method***

Display a prompt box which ask the user for her/his name, and output a message:

```
<!DOCTYPE html>
<html>
<body>

<p>Click the button to demonstrate the prompt box.</p>

<button onclick="myFunction()">Try it</button>

<p id="demo"></p>

<script>
function myFunction() {
  var person = prompt("Please enter your name", "Harry Potter");
  if (person != null) {
    document.getElementById("demo").innerHTML =
    "Hello " + person + "! How are you today?";
  }
}
</script>

</body>
</html>
```