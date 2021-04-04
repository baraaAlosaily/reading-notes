# Opertions and loop 

![loop](https://res.cloudinary.com/practicaldev/image/fetch/s--3gD4biUG--/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://dev-to-uploads.s3.amazonaws.com/i/ws2zjx0flaay4jxmtwnv.png)

## comparison operations:

### Evaluation condtion 
We have to understand logical operations that assigned int the JS 

![op](https://slideplayer.com/slide/15945194/88/images/25/Logical+Operators+%28cont.%29.jpg)

![p](https://i.ytimg.com/vi/wFB-ywsNPwg/maxresdefault.jpg)


***Examples***

Not equal value
```
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Comparison</h2>

<p>Assign 5 to x, and display the value of the comparison (x !== 5):</p>

<p id="demo"></p>

<script>
var x = 5;
document.getElementById("demo").innerHTML = (x !== 5);
</script>

</body>
</html>
```
Less than or equal to 
```
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Comparison</h2>

<p>Assign 5 to x, and display the value of the comparison (x <= 8).</p>

<p id="demo"></p>

<script>
var x = 5;
document.getElementById("demo").innerHTML = (x <= 8);
</script>

</body>
</html>
```

And 
```
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Comparison</h2>

<p>The AND operator (&&) returns true if both expressions are true, otherwise it returns false.</p>

<p id="demo"></p>

<script>
var x = 6;
var y = 3;

document.getElementById("demo").innerHTML = 
(x < 10 && y > 1) + "<br>" + 
(x < 10 && y < 1);
</script>

</body>
</html>
```

## For loop

Loops can execute a block of code a number of times

Syntax

```
for (statement 1; statement 2; statement 3) {
  // code block to be executed
}
```

Statement 1 is executed (one time) before the execution of the code block.

Statement 2 defines the condition for executing the code block.

Statement 3 is executed (every time) after the code block has been executed.


***Example***
```
<p id="demo"></p>

<script>
var cars = ["BMW", "Volvo", "Saab", "Ford"];

var i = 0;
var len = cars.length;
var text = "";

for (; i < len; ) {
  text += cars[i] + "<br>";
  i++;
}
document.getElementById("demo").innerHTML = text;
</script>

</body>
</html>
```

Output

```
BMW
Volvo
Saab
Ford
```

## While loop

The while loop loops through a block of code as long as a specified condition is true.

```
while (condition) {
  // code block to be executed
}
```

***Example***

<!DOCTYPE html>
<html>
<body>

<h2>JavaScript While Loop</h2>

<p id="demo"></p>

<script>
var text = "";
var i = 0;
while (i < 10) {
  text += "<br>The number is " + i;
  i++;
}
document.getElementById("demo").innerHTML = text;
</script>

</body>
</html>
```

Summary

+ Conditional statements allow your code to make decisions about what to do next.
+ Comparison operators (===, ! ==, ==, ! =, <, >, <=, =>)are used to compare two operands.
+ Logical operators allow you to combine more than one set of comparison operators.
+ Data types can be coerced from one type to another.
+ All values evaluate to either truthy or falsy.
+ There are three types of loop: for, while, and do ... while. Each repeats a set of statements.




