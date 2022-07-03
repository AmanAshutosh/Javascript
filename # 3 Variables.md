# Javascript Variables

4 Ways to Declare a JavaScript Variable:
* Using var
* Using let
* Using Const
* Using nothing

# What are Variables?
Variables are containers for storing data (storing data values).
In this example, x, y, and z, are variables, declared with the var keyword:

    var x = 5;
    var y = 6;
    var z = x + y;

In this example, x, y, and z, are variables, declared with the let keyword:
    
    let x = 5;
    let y = 6;
    let z = x + y;
    
In this example, x, y, and z, are undeclared variables:
    
    x = 5;
    y = 6;
    z = x + y;
    
From all the examples above, we can guess:
* x stores the value 5
* y stores the value 6
* z stores the value 11

# When to Use JavaScript var?
Always declare JavaScript variables with var,let, or const.<br>
The var keyword is used in all JavaScript code from 1995 to 2015.<br>
The let and const keywords were added to JavaScript in 2015.<br>
If you want your code to run in older browser, you must use var.<br>

# When to Use JavaScript const?
If we want a general rule: always declare variables with const.<br>
If we think the value of the variable can change, use let.<br>
In this example, price1, price2, and total, are variables:<br>

    const cost1 = 5;
    const cost2 = 6;
    let total = cost1 + cost2;
    
The two variables price1 and price2 are declared with the const keyword.
These are constant values and cannot be changed.
The variable total is declared with the let keyword.
This is a value that can be changed.

Just like in algebra, variables hold values:

    let x = 5;
    let y = 6;
    
Just like in algebra, variables are used in expressions:

    let z = x + y;
From the example above, we can guess that the total is calculated to be 11.
# Note
* Variables are containers for storing values.
* It's a good programming practice to declare all variables at the beginning of a script.
* If you put a number in quotes, the rest of the numbers will be treated as strings, and concatenated. ( let x = 2 + 3 + "5"; )

# How to Use JavaScript Variables in Functional Scope
A variable declared inside a function using these keywords is not accessible outside the function. That's the applied functional scope.
It is true irrespective of whether we use var, let, or const. Inside the function, they are pretty similar in managing a variable's scope.
Let's take an example again:

    // f1() is a function

    function f1() {
    let name = "codelessness";
    const ZIP = 844502;
    var age = 25;   
    }

    f1();

    console.log(name); // Uncaught ReferenceError: name is not defined
    console.log(ZIP);  // Uncaught ReferenceError: ZIP is not defined
    console.log(age);  // Uncaught ReferenceError: age is not defined

As we see above, none of the variables are accessible outside of the function, not even age which is declared using var. So, the conclusion is,

    The variable declared with var inside a function is not accessible outside of it. The keyword var has function-scope.
    
 # How to Use JavaScript Variables in Global Scope
 Variables declared outside of any functions and blocks are global and are said to have Global Scope. This means we can access them from any part of the current JavaScript program.

we can use *var, let, and const* to declare global variables. But we shouldn't do it too often.
    
    let name = "codelessness";
    const ZIP = 844502;
    var age = 25;  

    // f1() is a function
    function f1() {
      console.log(name); // codelessness
      console.log(ZIP);  // 844502
      console.log(age);  // 25
    }

    f1();

    console.log(name); // codelessness
    console.log(ZIP);  // 844502
    console.log(age);  // 25

As we see, the variables are accessible everywhere.
So, to restrict the scope of a variable using the var, let, and const keywords, here's the order of accessibility in scope starting with the lowest:
* var: The functional scope level
* let: The block scope level *(we will discuss this  separately )*
* const: The block scope level *(we will discuss this  separately )*

![scope img](https://drive.google.com/file/d/1AL5bDdLOTVv_9uB9mgBnjU4xZ-H9x-OQ/view?usp=sharing)





# Conclusion 
So we learned about Variables in Javascript.
Thankyou, If you loved this do share it with your friends.
 
