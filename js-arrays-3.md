# .map() function

.map() is called on an array, it takes an argument of a callback function and returns a new array! Take a look at an example of calling .map()

``` javascript

let numbers = [1, 2, 3, 5, 7, 11];
const mapArray = numbers.map(function(x){ return x*2; })
console.log(mapArray); // expected output: [2, 4, 6, 10, 14, 22]

```

# Task 1: Write a program to shallow copy an array.

Input Format: An array of size n.

Output Format: Copied array of size n.

``` javascript

function shallowCopy(input) {
  let newMessages = input.map((m) => m);
  return newMessages;
}

```
