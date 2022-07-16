# JavaScript Let
* The let keyword was introduced in ES6 (2015).
* Variables defined with let cannot be Redeclared.
* Variables defined with let must be Declared before use.
* Variables defined with let have Block Scope.

# Cannot be Redeclared
With let we can not do this

    let x = "codelessness";
    let x = 0;

    // SyntaxError: 'x' has already been declared
    
With var we can:

    var x = "codelessness";
    var x = 0;
    // Output will be 0
    
so now here comes *SCOPE*. 
# What is a scope?
A block (that is, a code block) is a section of the code we define using a pair of curly brace s({...}). 
Something like this:

    {
      let name = "codelessness";
    }
    
 Usually, we define a function using the function keyword and a name. 
 Just be aware that we can define a function without a name, which we call an 'anonymous function'.
 But we won't discuss that now for simplicity.
 Here is a function with the name test.
 
    function check() {
       let name = "alex";
    }
    
Anything and everything outside of a block or a function we'll call Global. 
So, when we declare variables, they can exist within a block, inside a function, or outside of a block/function – that is, they have global scope.
There are mainly three types of scope:
* Block Scope 
* Function Scope
* Global Scope

The three keywords *var, let, and const* work around these scopes. So let's understand how things fit together.
If we do not want a variable declared inside a { } block to be accessed outside of the block, 
we need to declare them using the let or const keywords. Variables declared with the var keyword inside the { } block are accessible outside of the block too.
So, be careful.
For Example:

    {
    let name  = 'codelessness';
    const ZIP = 844502;
    var age = 25;
    }

    console.log(f_name); // Uncaught ReferenceError: f_name is not defined
    console.log(ZIP);  // Uncaught ReferenceError: ZIP is not defined.
    console.log(age);  // 25
  
As we can see, the value of the age variable may get overridden unknowingly and eventually introduce a bug. So, the moral of the story is
    
    Do not use the 'var' keyword inside a block (block scope). Always use 'let' and 'const' instead.
    
This is all for *let* we will dive deep in let,const and var soon. 

# conclusion 
In this we learned about let keyword and its working, and some details about scope too.
We will deep dive in these topics once we are done with the basic introduction. 
Till *just code it* :)
