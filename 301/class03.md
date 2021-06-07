## What does .map() return?
 - ### return a New array of the same length as the original array
## If I want to loop through an array and display each value in JSX, how do I do that in React?

 - ### we can put any valid JavaScript expression inside the curly braces in JSX.

## Each list item needs a unique **key**.

## What is the purpose of a key?

 - ### Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity:

---

## What is the spread operator?

 - ### spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.

## List 4 things that the spread operator can do.

 - ### Copying an array
 - ### Using Math functions
 - ### Adding an item to a list
 - ### Adding to state in React

## Give an example of using the spread operator to combine two arrays.

 - ### const arr1 = [1,2,3]
 - ### const arr2 = [4,5,6]
 - ### const arr3 = [...arr1, ...arr2] 

## Give an example of using the spread operator to add a new item to an array.

 - ### const arr1 = [1,2,3]
 - ### const arr2 = [4,5,6,...arr1]

## Give an example of using the spread operator to combine two objects into one.

 - ### const obj1 = {first: "1"}
 - ### const obj2 = {second: "2"}
 - ### const obj3 = {...arr1, ...arr2}

---

## In the video, what is the first step that the developer does to pass functions between components?

 - ### create the function wherever the state is.

## In your own words, what does the increment function do?
 - ### it will take a name and loop through the ppl object and if it's matching it will increase the count for this name.

## How can you pass a method from a parent component into a child component?
## How does the child component invoke a method that was passed to it from a parent component?

 - ### inside the component as we did in the other data put we will use this.**the function name** and we will use invoke in the child this.props.**the name we gave it when we pass it**




