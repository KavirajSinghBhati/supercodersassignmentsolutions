# JS: Object Methods

An object in JavaScript may also have a function as a member, in which case it 
will be known as a method of that object.

Let us see such an example :

```javascript
let school = {
  name: 'CodeQuotient ',
  location : 'Mohali',
  established : 2015,
  displayInfo : function(){
    console.log(`${school.name} was established 
       in ${school.established} at ${school.location}`);
  }
}
school.displayInfo();
```

In the above example, “displayinfo” is a method of the school object that is 
being used to work with the object’s data, stored in its properties.

## “this” in methods:-

It’s common that an object method needs to access the information stored in the object to do its job.

For instance, the code inside school.displayInfo() may need the name of the school.

To access the object, a method can use this keyword.

The value of this is the object “before dot”, the one used to call the method.

```javascript
let school = {
  name: 'CodeQuotient ',
  location : 'Mohali',
  established : 2015,
  displayInfo : function(){
    console.log(`${this.name} was established 
       in ${this.established} at ${this.location}`);
  }
}
```

## Task 1: Implement below mentioned methods on the given object named ladder.

    setSteps :- takes no. of steps as a parameter, and set the steps accordingly.
    getSteps :- return the no. of steps.
    stepUp :- Increase the no. of steps by 1.
    stepDown :- Decrease the no. of steps by 1.

```javascript

const ladder = {
	steps: 0
};

ladder.setSteps = function(steps){
  this.steps = steps;
}

ladder.getSteps = function() {
  return this.steps;
}

ladder.stepUp = function() {
  this.steps = this.steps + 1;
}

ladder.stepDown = function() {
  this.steps = this.steps - 1;
}
```
