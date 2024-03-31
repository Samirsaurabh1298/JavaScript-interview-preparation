***1)When will we click on button background color should be change. How many ways to do it ***

```js

<div>
 <button onClick="changeColor('red')">Red</button>
 <button onClick="changeColor('yellow')">Yellow</button>
 <button onClick="changeColor('purple')">Purple</button>
</div>

function changeColor(color) {
    document.body.style.backgroundColor = color;
}
```