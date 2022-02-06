# The .pop() Method :-

The pop() method removes the last element from an array.

# The .push() Method :-

The push() method adds a new element to an array (at the end)

# The .shift() Method :-

Shifting is equivalent to popping, working on the first element instead of the last.

The shift() method removes the first array element and "shifts" all other elements to a lower index.

# The .unshift() Method :-

The unshift() method adds a new element to an array (at the beginning), and "unshifts" older elements.

# The .splice() Method :-

The splice() method can be used to add new items to an array.

``` javascript

let friends = [ "Sumit", "Pawan" , "Paras" ];
friends.splice(2, 0, "Amit", "Amar"); // [ "Sumit", "Pawan" , "Amit", "Amar" , "Paras" ]

```
The first parameter (2) defines the position where new elements should be added (spliced in).

The second parameter (0) defines how many elements should be removed.

The rest of the parameters ("Amit", "Amar") define the new elements to be added.

The splice() method returns an array with the deleted items. You can use splice() to remove elements.

``` javascript

var friends = [ "Sumit", "Pawan" , "Amit", "Amar" , "Paras" ]
friends.splice(0, 2); // ["Amit", "Amar" , "Paras"]

```

The first parameter (0) defines the position where new elements should be added (spliced in).

The second parameter (2) defines how many elements should be removed.

The rest of the parameters are omitted. No new elements will be added.

# Task 1: What will be the output of below code snippet.

``` javascript

const arr = [];
arr.push(5);
arr.push(21);
arr.push(89);
arr.push([2, 71]);
arr.push(31);
arr.splice(3, 0, [40, 99]);
arr.pop();
arr.shift();
arr.splice(1, 1);
arr.unshift(999);
console.log(arr);

```

Output : [ 999 21 [40 99] [2 71] ]
