var, let, and const are keywords used in JavaScript for declaring variables.

-----------------------SCOPE)->How variable works in scope.-----------------------------------------------
• Var:- Var has a *function and global scope*, This means a variable declared with var can be accessed throughout the function.

• Let and Const have a block scope , this means they are only accessible within the Block of code.
for Example--- (like an if statement or a loop).


------------------------------------------------REASSIGNMENT----------------------------------------------
• VAR and LET can be reassigned a new value after they are declared.

• CONST- We Cannot be reassigned a new value after it's declared. const value can't change.


---------------------------------------------------HOISTING-----------------------------------------------
• VAR:- Declarations are hoisted to the top of their scope (function or global),but its value will be undefined.

• LET and CONST: Declarations are also hoisted, but not initialized. Trying to use a let or const  variable before it's declared will result in a Reference Error.
