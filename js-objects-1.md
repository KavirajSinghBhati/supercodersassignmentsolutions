# JS Objects

Objects in JavaScript, just as in many other programming languages, can be compared to objects in real life. 
The concept of objects in JavaScript can be understood with real life, tangible objects.

In JavaScript, an object is a standalone entity, with properties and type. Compare it with a cup, for example. 
A cup is an object, with properties. A cup has a color, a design, weight, 
a material it is made of, etc. The same way, JavaScript objects can have properties, which define their characteristics.

An object can be created with figure brackets {…} with an optional list of properties. 
A property is a “key: value” pair, where key is a string (also called a “property name”), 
and value can be anything.These keys can be variables or functions and are called 
properties and methods, respectively, in the context of an object.

An empty object (“empty cabinet”) can be created using one of two syntaxes below.

```javascript
let user = new Object(); // "object constructor" syntax
let user = {}; // "object literal" syntax
```

We can immediately put some properties into {...} as “key: value” pairs.

```javascript
let user = {   // an object
 name: "Rohan", // by key "name" store value "Rohan"
 age: 21    // by key "age" store value 21
};
```

In the user object, there are two properties:

The first property has the name "name" and the value "Rohan".

The second one has the name "age" and the value 21.

We can add, remove and read data from it any time.

To remove a property, we can use delete operator.

```javascript
delete user.age;
```

We can also use multiword property names, but then they must be quoted.


```javascript
let user = {
 name: "Rohan",
 "like games": true // multiword property name must be quoted
};
```

## Object with const can be changed

Please note: an object declared as const can be modified.

For instance

```javascript
const user = {
 name: "Rohan"
};
 
user.name = "Mohan"; // (1)
 
alert(user.name); // Pete
```

It might seem that the line (1) would cause an error, but no. The const fixes the value of user, but not its contents.

The const would give an error only if we try to set user=... as a whole.

When we pass a variable assigned to an object into a function as an argument, the computer interprets the parameter name as 
pointing to the space in memory holding that object. As a result, functions which 
change object properties actually mutate the object permanently (even when the object is assigned to a const variable).

For multiword properties, the dot access doesn’t work:

```javascript
user.like games= true // syntax error
```

The dot requires the key to be a valid variable identifier. 
That implies: contains no spaces, doesn’t start with a digit and doesn’t include special 
characters ($ and _ are allowed).There’s an alternative “square bracket notation” that works with any string.

```javascript
let user = {};
 
// set
User["like games"] = true;
 
// get
alert(user["like games"]); // true
 
// delete
delete user["like games"];
```

Square brackets also provide a way to obtain the property name as the result 
of any expression – as opposed to a literal string – like from a variable as follows

```javascript
let key = "like games"
user[key] = true;
```

## Testing Object for property :-

Sometimes it is useful to check if the property of a given object exists or not. 
We can use the .hasOwnProperty(propname) method of objects to determine if that object has the given property name. 
.hasOwnProperty() returns true or false if the property is found or not.

Example:

```javascript
var myObj = {
 top: "hat",
 bottom: "pants"
};
myObj.hasOwnProperty("top");  // true
myObj.hasOwnProperty("middle"); // false
```

## Accessing Nested Objects :-

The sub-properties of objects can be accessed by chaining together the dot or bracket notation.

Here is a nested object:


```javascript
var ourStorage = {
 "desk": {
  "drawer": "stapler"
 },
 "cabinet": {
  "top drawer": {
   "folder1": "a file",
   "folder2": "secrets"
  },
  "bottom drawer": "soda"
 }
};
ourStorage.cabinet["top drawer"].folder2; // "secrets"
ourStorage.desk.drawer; // "stapler"
```

## Accessing Nested Arrays :-

Objects can contain both nested objects and nested arrays. 
Similar to accessing nested objects, Array bracket notation can be chained to access nested arrays.

Here is an example:


```javascript
var ourPets = [
 {
  animalType: "cat",
  names: [
   "Meowzer",
   "Fluffy",
   "Kit-Cat"
  ]
 },
 {
  animalType: "dog",
  names: [
   "Spot",
   "Bowser",
   "Frankie"
  ]
 }
];
ourPets[0].names[1]; // "Fluffy"
ourPets[1].names[0]; // "Spot"
```


# Task 1: What will be the return value of below function calls.


```javascript
const rentalCar = {
    manufacturer: 'Tata',
    model: 'Altroz',
    seatingCapacity: 4,
    ratePerKilometer: 10,
    hourlyRate: 1200,
    carRegNumber: 'CH04AE0000',
    bookings: [
        {
            bookingId: '1',
            customer: {
                name: 'ABC',
                contact: '+91-09876-54321'
            },
            kmsTravelled: 432,
            billedAmount: 4500,
            pickupAddress: '15/34, somewhere, some state, some country'
        },
        {
            bookingId: '2',
            customer: {
                name: 'DEF',
                contact: '+91-056321-54789'
            },
            kmsTravelled: 220,
            billedAmount: 2500,
            pickupAddress: '74/10, nowhere, another state, some country'
        },
    ],
    driverDetails: {
        name: 'XYZ',
        contact: '+91-12345-67890'
    },
};
```

Note: please use dot notation to access properties in questions, and end statements with semi-colon(;). eg. rentalCar.model;

- How would you access the driver's name of rentalCar object?
  ```javascript
  rentalCar.driverDetails.name;
  ```
- How would you delete hourlyRate property from rentalCar object?
  ```javascript
  delete rentalCar.hourlyRate;
  ```
- How would you access the 2nd booking's customer name from rentalCar object?
  ```javascript
  rentalCar.bookings[1].customer.name;
  ```
