# Day-3 

## Array methods
### Array slice()
    Slicing is the operation of extracting a contiguous portion (a sub-sequence) of an array or list into a new array, without modifying the original. The portion is specified by a start index and an end index.

#### Array splice()
    Splice is an operation that changes an array in place by removing, replacing, or inserting elements at a given position. It is a mutating method: it modifies the original array and returns an array containing the elements that were removed.

#### Array toString()
    toString() is a method that returns a string representation of a value. It is defined on Object.prototype, so almost every object in JavaScript inherits it, and many built-in types (Array, Number, Date, Function, etc.) override it to provide a meaningful result.

#### Array at()
    at() is a method that returns the element at a given index, and it accepts negative integers to count backward from the end. It was introduced in ES2022 and exists on Array, String

#### Array join()
    join() is an Array method that concatenates all elements of an array into a single string, placing a specified separator between each element. It is non-mutating: the original array is unchanged, and the result is always a string.

#### Array push()
    push() is an Array method that adds one or more elements to the end of an array and returns the new length of the array. It is a mutating method: it modifies the original array in place.

#### pop()
    pop() is an Array method that removes the last element from an array and returns that removed element. It is a mutating method: it modifies the original array in place and reduces its length by one.

#### Array shift()
    shift() is an Array method that removes the first element from an array and returns that removed element. It is a mutating method: it modifies the original array in place, reduces its length by one, and re-indexes every remaining element (each moves one position to the left)

#### Array unshift()
    unshift() is an Array method that adds one or more elements to the beginning of an array and returns the new length of the array. It is a mutating method: it modifies the original array in place and shifts every existing element to a higher index

#### Array delete()
    JavaScript has no Array.prototype.delete() method. arr.delete(1) throws TypeError: arr.delete is not a function.

#### Array concat()
    concat() is a method on Array (and String) that merges two or more arrays (or values) into a new array without changing the originals. It is non-mutating and returns a new array containing the elements of the original followed by the arguments.



## Array Search Methods
#### Array indexOf()
    indexOf() is a method on Array (and String) that searches for a given element and returns the index of its first occurrence, or -1 if it is not found. It is non-mutating: the original array is unchanged.

#### Array lastIndexOf()
    lastIndexOf() is a method on Array (and String) that searches backward from the end and returns the index of the last occurrence of a given element, or -1 if it is not found. It is non-mutating, and on arrays it compares using strict equality (===)

#### Array includes()
    includes() is a method on Array (and String) that checks whether a value exists and returns a boolean: true if found, false otherwise. It is non-mutating

#### Array find()
    find() is an Array method that returns the first element that satisfies a given testing function, or undefined if no element matches. It is non-mutating

#### Array findIndex()
    findIndex() is an Array method that returns the index of the first element that satisfies a given testing function, or -1 if no element matches. It is non-mutating, short-circuits at the first match,


## Array Sort Methods
### Alphabetic Sort
#### Array sort()
    sort() is an Array method that sorts the elements of an array in place and returns a reference to the same array. It is a mutating method. With no arguments, it converts elements to strings and sorts them by UTF-16 code unit order, which is why numbers sort incorrectly by default.

#### Array reverse()
    reverse() is an Array method that reverses the order of the elements of an array in place and returns a reference to the same array. The first element becomes the last, and the last becomes the first. It is a mutating method

#### Sorting Objects
    Sorting objects means ordering an array of objects by the value of one or more of their properties, using Array.prototype.sort() with a comparator function. Objects cannot be sorted with the default sort(), because it converts them to strings ("[object Object]"), so every object looks identical and the order does not change meaningfully.

    sort() is mutating and stable (guaranteed since ES2019). For non-mutating sorting, use toSorted() or [...arr].sort().

### Numeric Sort
#### Numeric Sort
    Numeric sort means ordering an array of numbers by their numeric value (for example 1, 2, 10) instead of by their string representation ("1", "10", "2"). In JavaScript it requires passing a comparator function to sort(), because the default sort() converts every element to a string and compares UTF-16 code units.

    or

    "Array.sort() sorts values as strings by default. To sort numbers correctly, I provide a comparator such as (a, b) => a - b for ascending order and (a, b) => b - a for descending order."

 #### Random Sort
    "sort() normally sorts an array based on a comparison function. When I use Math.random() - 0.5, the comparison function randomly returns a positive or negative value, so the elements get rearranged randomly

 #### Math.min() & Math.max()
    "Math.min() is used to find the smallest value and Math.max() is used to find the largest value. When working with an array, I use the spread operator to pass the array elements as individual arguments."