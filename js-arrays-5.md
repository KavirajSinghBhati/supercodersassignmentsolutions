# .filter() function

The filter() method creates a new array with all elements that pass the test implemented by the provided function.

``` javascript
let ageArray = [45, 4, 9, 16, 25];
let over18 = ageArray.filter(function (age) {
 return age > 18;
});
Console.log ( over18 ) // [ 45, 25 ]
```

Age > 18; is the condition in the callback function. Any age from the ageArray that’s value is greater than 18 will be added to the over18 array.


# Task 1: Write a program to remove all even numbers from an array.

Input Format: An array of size n.

Output Format: Return an array containing only odd numbers. If none return an empty array.

``` javascript

function removeEven(input) {
  return input.filter(num => num % 2 != 0);
}

```
