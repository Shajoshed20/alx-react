# 0x06. React Immutable

## General Learning Objectives

* Immutable objects. Who, what, when, where, and why?
* How to use the Immutable.js library to bring immutability to Javascript
* The differences between List and Map
* How to use Merge, Concat, and Deep Merging
* What a lazy Seq is

## Tasks 

* Task 0 - Copy the necessary config files specified in the description to the root directory of the project and execute npm install.

In a file named 0-fromjs.js, create a function getImmutableObject that accepts object as a parameter and converts it into an immutable Map using fromJS of the Immutable.js library

* Task 1 - In 1-map.js, modify the function getImmutableObject using Map from Immutable.js

* Task 2 - Given the function below, edit it to return the value of the object at the defined path

    `export default function accessImmutableObject(object, array) {`
    `}`

    - The first argument is a plain object
    - The second one is an array containing a list of a path to some key in the object
    - The function should return the value of the object at the defined path

* Task 3 - In file 3-list.js, create these 2 functions:

    `export function getListObject(array) {`
    `}`

    `export function addElementToList(list, element) {`
    `}`
    - getListObject accepts an array as parameter and converts it into an immutable List using the Immutable.js library
    - addElementToList accepts two arguments: first one is a List and second one is a string
        - append the string to the list and return the list

* Task 4 - Create & export a constant named map. It should create an Immutable Map with the following object:

    `{`
        ` 1: 'Liam',`
        ` 2: 'Noah',`
        ` 3: 'Elijah',`
        ` 4: 'Oliver',`
        ` 5: 'Jacob',`
        ` 6: 'Lucas',`
    `}`
    Export a second constant named map2. It should use the first map and modify the following values:

    - Modify the value for the index 2, to Benjamin
    - Modify the value for the index 4, to Oliver

* Task 5 - Create a function named concatElements
    - It accepts two arguments page1 and page2. Both are arrays
    - It should return a List containing the values of the two pages

    Create a function named mergeElements
    - It accepts two arguments page1 and page2. Both are objects
    - It should return a List containing the values of the two pages
    - If two values are the same, page2 values should be used.

* Task 6 - 