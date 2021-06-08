# Passing Functions as Props

### list and keys

- What does .map() return?
  Map(): returns an new array with changes but with the same length.

- If I want to loop through an array and display each value in JSX, how do I do that in React?
  I will use map(). to loop throught the array

- Each list item needs a unique ID.

- What is the purpose of a key?
  It help React to identify which items have changed, are added, or are removed. they should be given to the elements inside the array to give the elements a stable identity.

spread operator

- What is the spread operator?
  The three dot `(...)`, to expand an iterable object into the list of arguments.
- List 4 things that the spread operator can do.
  1.Concatenating or combining arrays.
  2.Copying an array.
  3.Adding to state in React.
  4.Adding an item to a list.

- Give an example of using the spread operator to combine two arrays.

```
const arrayOfAges = [20,35,40];
const arrayOfHieghts = [158, 160, 187];
const combineArrays = [...arrayOfAges, ...arrayOfHieghts] //Combining two arrays using spread operator
```

- Give an example of using the spread operator to add a new item to an array.

```
let numberStore = [0, 1, 2];
let newNumber = 12;
numberStore = [...numberStore, newNumber];
```

- Give an example of using the spread operator to combine two objects into one.

```
const object1 = {};
const object2 = {};
const combineObjects = [...object1, ...object2] //Combining two arrays using spread operator
```

## How to Pass Functions Between Components

- In the video, what is the first step that the developer does to pass functions between components?
  creating a function

- In your own words, what does the increment function do?
  It is function modified the objects passing the objects, find the matching objects and update that

- How can you pass a method from a parent component into a child component?
  write the method inside the render -> return component then call it where ever you want

- How does the child component invoke a method that was passed to it from a parent component?
  write the method inside the render -> return component then call
