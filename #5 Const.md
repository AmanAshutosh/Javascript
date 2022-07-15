# JavaScript Const
* The const keyword was introduced in ES6 (2015).
* Variables defined with const cannot be Redeclared.
* Variables defined with const cannot be Reassigned.
* Variables defined with const have Block Scope.

A const variable cannot be reassigned:

    const PI = 3.141592653589793;
    PI = 3.14;      // This will give an error
    PI = PI + 10;   // This will also give an error.
    
JavaScript const variables must be assigned a value when they are declared:

    // Incorrect
    const PI;
    PI = 3.14159265359;
    
    Correct
    const PI = 3.14159265359;
    
# When to use JavaScript const?
As a general rule, always declare a variable with const unless you know that the value will change.
Use const when you declare:
* A new Array
* A new Object
* A new Function
* A new RegExp

# Constant Objects and Arrays
The keyword const is a little misleading.
It does not define a constant value. It defines a constant reference to a value.
Because of this we can NOT:

* Reassign a constant value
* Reassign a constant array
* Reassign a constant object
But we can:

Change the elements of constant array
Change the properties of constant object
we can change the elements of a constant array:

    // we can create a constant array:
    const cars = ["Saab", "Volvo", "BMW"];

    // we can change an element:
    cars[0] = "Toyota";

    // we can add an element:
    cars.push("Audi");
But we can NOT reassign the array:

    const cars = ["Saab", "Volvo", "BMW"];
    cars = ["Toyota", "Volvo", "Audi"];    // ERROR
    
# Constant Objects
we can change the properties of a constant object:

    // we can create a const object:
    const car = {type:"Maruti", model:"500", color:"white"};

    // we can change a property:
    car.color = "yellow";

    // we can add a property:
    car.owner = "golu";
    
But we can NOT reassign the object:

    const car = {type:"Maruti", model:"500", color:"white"};
    car = {type:"Volvo", model:"EX60", color:"red"};    // ERROR.
