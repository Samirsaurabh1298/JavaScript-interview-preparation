***1)What is the difference between == and === in js:***
``` js
 == and === both are comparison operation.
 == only compare value.
 === copares value and types. 

if('1'== 1){
     //only value
};


if('1' === 1){
    //value and types
};

```

***2)What is difference between NULL and UNDEFINED.***
```js
⨀ They both represent empty value, but diffrence is that when u define a variable and not assign a value to it. it automaticly take a placeholder called <b>UndefIned</b>

⨀ If we try to access typeOf <b>Null</b>  we will get object.

```

***3)What is CLOSURE:***
```js
function bundled along with it's lexical scope is called closure.
Example:-
function outerFunction(outerVariable){
    function innerFunction(innerVariable){
        console.log('OuterVariable:', outerVariable)
        console.log('InnerVariable:', innerVariable)
    }
    return innerFunction;
}

const result = outerFunction("Hello")
result("Cloure")
```
***4)What is PROMISE:***
```js
*A promise is an object representing the eventual completion or failure of an asynchronous operation. is called promise.

*It allows you to handle asynchronous operations more easily and avoid callback hell by chaining .then() and .catch() methods.

*A promise can be in three states: pending, fulfilled, or rejected.
```
