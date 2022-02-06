# .forEach() function

forEach() calls a provided callback function once for each 
element in an array in ascending order. It is not invoked for index properties that have been deleted or are uninitialized.

``` javascript

let numbers = [2, 3, 5, 7, 9, 11];
numbers.forEach(myFunction);
 
function myFunction(value, index, array) {
 console.log(`${arr[index]} = ${value}`)
}
```

callback is invoked with three arguments

- the value of the element
- the index of the element
- the Array object being traversed
    
The range of elements processed by forEach() is set before the first invocation of callback. 
Elements which are appended to the array after the call to forEach() begins will not be visited by callback. 
If elements that are already visited are removed (e.g. using shift()) 
during the iteration, later elements will be skipped.The return value for .forEach() will always be undefined.

# Task 1: Write a program to add 1 to each element of input array.

Input Format: An array of size n.

``` javascript

function addOneToEach(input) {
  input.forEach((v, i, a) => a[i]++);
}

```
