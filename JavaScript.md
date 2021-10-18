# JavaScript

## Basics
### Syntax & Semantics
#### Variables
Using the keyword 'var', you declare the variable name and assign it an inital value.
```Javascript
Var MyName = "Seth";
console.log(MyName);
```
Using the keyword 'let' will create a immutable variable which has block scope
```Javascript
let PI = 3.1415;
console.log(PI);
```
Using the keyword 'const' will create a variable which is similar to let however it's properties can be change.
```Javascript
const MyCar = {Type:"Hatchback", Make:"Hyundai", Owner:"Bobby"};
MyCar.Owner = "Seth";
```

Creating objects can be done by using {}, like in the example above, the MyCar Object.

#### Operators
Usual mathmathic operators: + - * / ** %

Increment and decrement: -- ++

And assignment with an operator: +=, -=, *=, /=

Comparing variables by doing:
```Javascript
var foo = 7
var bar = "7"
//Check if the value matches
if(foo == bar){
  console.log("foo == bar")
}
//Check if the value and type matches
if(foo === bar){
  console.log("foo === bar")
}
```



You can create functions using the 'Function' keyword:
```Javascript
function Product(x, y){
  return x * y
}
```
### Built in Data Structures
JS has few data structures built into it.
### Arrays
Dynamic arrays in JS where you can add and remove elements.
Not restricted to 1 type of data within an array: Can store strings, doubles, objects in one structure.

```Javascript
let vehicles = ["Planes", "Trains", "Automobiles"]
vehicles.push("Bikes")
console.log(vehicles)
```
### Sets
Similar to arrays but order does not matter and only keeps unique items.
```Javascript
let ID = new Set("001", "002", "003", "004")
ID.add("005")     //Adds 005 to the set
ID.delete("003")  //Removes 003 from the set
ID.add("001")     //Goes to add 001 to the set, no duplicates so nothing changes
console.log(ID)
```
### Maps
Contains an array of key:value pairs
```Javascript
const fruits = new Map([
  ["Apples", 2.35],
  ["Grapes", 4.45],
  ["Cherries", 4.80]
]);
```
Can also be created by using *MapName*.set(x, y)

### Objects
Everything but primitive data types(String, Number, Boolean, Null, Undefined) are considered objects, including functions.
Objects are made up of properties which have a name and value.
```Javascript
const MyCar = {Type:"Hatchback", Make:"Hyundai", Owner:"Bobby", 
  toString: function(){Return this.Make + " " + this.Type + " is owned by" + this.Owner;}
  };
```
## How JS works & Using JS

### Under the hood

### Supported Paradigms 


## Advanced




## Interesting Libraries




## Sources
<details><summary>w3schools</summary>

  https://www.w3schools.com/js/js_variables.asp
  
  https://www.w3schools.com/js/js_let.asp

  https://www.w3schools.com/js/js_const.asp

  https://www.w3schools.com/js/js_arithmetic.asp

  https://www.w3schools.com/js/js_assignment.asp

  https://www.w3schools.com/js/js_datatypes.asp

  https://www.w3schools.com/js/js_functions.asp

</details>

<details><summary>Other</summary>
https://dev.to/kartik2406/built-in-data-structures-in-javascript-hhl
</details>
