What does .map() return?

It returns array

If I want to loop through an array and display each value in JSX, how do I do that in React?

You can do it by using map() it creates a new array from calling a function for every array element.

Each list item needs a unique.

“key”

What is the purpose of a key?

Keys help React identify which items have changed, are added, or are removed.

The Spread Operator
What is the spread operator?

The JavaScript spread operator (...) allows us to quickly copy all or part of an existing array or object into another array or object.

List 4 things that the spread operator can do.

Copying an array.

Concatenating or combining arrays

Using Math functions.

Using an array as arguments.

Give an example of using the spread operator to combine two arrays.

const arr1 =[1,2,3]

const arr2 =[4,5,6]

const combine= [...arr1 , …arr2]

Give an example of using the spread operator to add a new item to an array.

const arr1 =[1,2,3]

const arr2 =[4,5, …arr1]

Give an example of using the spread operator to combine two objects into one.

Const obj1 ={name : “ahmad”}

Const obj2 ={age : 22}

Const obj3 ={...obj1 , …obj2}