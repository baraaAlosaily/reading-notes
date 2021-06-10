## Putting it all together

1. How would you break a mock into a component heirarchy?

se the same techniques for deciding if you should create a new function or object. One such technique is the single responsibility principle. Since you’re often displaying a JSON data model to a user, you’ll find that if your model was built correctly, your UI (and therefore your component structure) will map nicely. That’s because UI and data models tend to adhere to the same information architecture.

2. What is the single responsibility principle and how does it apply to components?
   A component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents. Each component has its own job and properties distinguish it from the other.
3. What does it mean to build a ‘static’ version of your application?
   Its a way to build a version of our app that renders the data model
4. Once you have a static application, what do you need to add?
   Add State to make the UI interactive
5. What are the three questions you can ask to determine if something is state?
   Is it passed in from a parent via props? If so, it probably isn’t state.
   Does it remain unchanged over time? If so, it probably isn’t state.
   Can you compute it based on any other state or props in your component? If so, it isn’t state.
6. How can you identify where state needs to live?
   dentify every component that renders something based on that state.
   Find a common owner component (a single component above all the components that need the state in the hierarchy).
   Either the common owner or another component higher up in the hierarchy should own the state.
   If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.
