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
    
From all the examples above, you can guess:
* x stores the value 5
* y stores the value 6
* z stores the value 11

# When to Use JavaScript var?
Always declare JavaScript variables with var,let, or const.<br>
The var keyword is used in all JavaScript code from 1995 to 2015.<br>
The let and const keywords were added to JavaScript in 2015.<br>
If you want your code to run in older browser, you must use var.<br>

# When to Use JavaScript const?
If you want a general rule: always declare variables with const.<br>
If you think the value of the variable can change, use let.<br>
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
From the example above, you can guess that the total is calculated to be 11.
# Note
* Variables are containers for storing values.
* It's a good programming practice to declare all variables at the beginning of a script.
* If you put a number in quotes, the rest of the numbers will be treated as strings, and concatenated. ( let x = 2 + 3 + "5"; )


# Conclusion 
So we learned about Variables in Javascript.
Thankyou, If you loved this do share it with your friends.
 
