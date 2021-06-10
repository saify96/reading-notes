## How would you break a mock into a component heirarchy?

 - ### FilterableProductTable (orange): contains the entirety of the example
 - ### SearchBar (blue): receives all user input
 - ### ProductTable (green): displays and filters the data collection based on user input
 - ### ProductCategoryRow (turquoise): displays a heading for each category
 - ### ProductRow (red): displays a row for each product

## What is the single responsibility principle and how does it apply to components?

 - ### a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.

## What does it mean to build a ‘static’ version of your application?

 - ### we don't need to use the state 

## Once you have a static application, what do you need to add?

 - ### ReactDOM.render() to make changes

## What are the three questions you can ask to determine if something is state?

 - ### Is it passed in from a parent via props? If so, it probably isn’t state.
 - ### Does it remain unchanged over time? If so, it probably isn’t state.
 - ### Can you compute it based on any other state or props in your component? If so, it isn’t state.


## How can you identify where state needs to live?

 - ### Identify every component that renders something based on that state.
 - ### Find a common owner component (a single component above all the components that need the state in the hierarchy).
 - ### Either the common owner or another component higher up in the hierarchy should own the state.
