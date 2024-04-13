**What is the difference between *==* and *===* in js** <br>
⨀ *==* and *===* both are comparison operation.<br>
⨀ *==* only compare value.<br>
⨀ *===* copares value and types. <br>

```
if('1'== 1){
     //only value
};

<br>

if('1' === 1){
    //value and types
};

```
<br>

What is difference between <b>NULL</b> and <b>UNDEFINED</b>   <br> 
⨀ They both represent empty value, but diffrence is that when u define a variable and not assign a value to it. it automaticly take a placeholder called <b>UndefIned</b>. <br>

⨀ If we try to access typeOf <b>Null</b>  we will get object.

***2)What is CLOSURE:***
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
***2)What is PROMISE:***
```js
*A promise is an object representing the eventual completion or failure of an asynchronous operation. is called promise.

*It allows you to handle asynchronous operations more easily and avoid callback hell by chaining .then() and .catch() methods.

*A promise can be in three states: pending, fulfilled, or rejected.
```
