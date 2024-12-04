var, let, and const are keywords used in JavaScript for declaring variables.

**SCOPE->>>>>> How variable works in scope.** <br>
• Var:- Var has a *function and global scope*, This means a variable declared with var can be accessed throughout the function.

• Let and Const have a block scope , this means they are only accessible within the Block of code.
for Example--- (like an if statement or a loop).


**REASSIGNMENT->>>>>>** <br>
• VAR and LET can be reassigned a new value after they are declared.

• CONST- We Cannot be reassigned a new value after it's declared. const value can't change.

```
let a = 1;
a = 2;
console.log(a); 
we will get aoutput 2.

const a = 1;
a = 2;
console.log(a); 
we will get typeError.
```


**HOISTING->>>>>>** <br>
•VAR:- Declarations are hoisted to the top of their scope (function or global),but its value will be undefined.

• LET and CONST: Declarations are also hoisted, but not initialized. Trying to use a let or const  variable before it's declared will result in a Reference Error.


***What is execution context?***
```js
*when javascript engine scan the javascript file, it makes an environment called the execution context.
*Everything in JS happens inside this execution context. It is divided into two components.
1)Memory component ---->Variable environment    2)code component ----->Code of execution.

There are two phase is execution context.
1)Creation phase   2)Execution phase.

*javascript is a synchronous single threaded language. synchronous means in asynchronous order, and single threaded means one command at a time in a specific order.
```

***What is JS Web Api***
```js
These all are Browser API.
1) SetTimeout();
2) Dom API;
3) Fetch();
4) LoaclStorage;
5) Console.
6) Location
```