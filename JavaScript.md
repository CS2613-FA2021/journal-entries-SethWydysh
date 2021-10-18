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


## How JS works & Using JS

### Under the hood

### Supported Paradigms 


## Advanced




## Interesting Libraries




## Sources
<details><summary>w3schools</summary>
<p>
  https://www.w3schools.com/js/js_variables.asp
  
  https://www.w3schools.com/js/js_let.asp

  https://www.w3schools.com/js/js_const.asp

  https://www.w3schools.com/js/js_arithmetic.asp

  https://www.w3schools.com/js/js_assignment.asp

  https://www.w3schools.com/js/js_datatypes.asp

  https://www.w3schools.com/js/js_functions.asp
</p>
</details>

<details><summary>Other</summary>
<p>
</p>
</details>
