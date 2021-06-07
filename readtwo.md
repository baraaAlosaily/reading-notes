## React: Component Lifecycle Events

1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?
   ![new](https://miro.medium.com/max/2800/0*0saPKFiTUk6W3FYp)

Here we use componentDidMount() to connect to the YouTube API and get videos when the components is rendered. (so the render first)

2. What is the very first thing to happen in the lifecycle of React?
   Here we use componentDidMount() to connect to the YouTube API and get videos when the components is rendered.

the constructor is the first thing will happen

3. Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates
   What does componentDidMount do?

```
constructor
render()
componentDidMount()
React Updates
componentWillUnmount
componentDidMount (Links to an external site.)
```

is executed after the first render only on the client side. This is where DOM or state updates should occur. This method is also used for integration with other JavaScript frameworks and any functions with delayed execution such as setTimeout or setInterval. We are using it to update the state so we can trigger the other lifecycle methods.

## React & Props

What types of things can you pass in the props?
we can passing integers, arrays, objects, string.. etc.

1. What is the big difference between props and state?
   regarding to Props it’s like arguments in the function, when create component inside react and want to render it we can pass the props that we give, state is something inside the component
2. When do we re-render our application?
   we can change the state in the application.
3. What are some examples of things that we could store in state?
   we can store the following
   integers, arrays, objects, string..

## Things I want to know more about

1.More about properties of props
