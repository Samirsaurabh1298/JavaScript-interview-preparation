***1)Write a JavaScript function to calculate the sum of two numbers.*** 
```
  function calculateTwoNum(a,b) {
    return a + b;
  }
  console.log(calculateTwoNum(2,3))
```

***2)Write a JavaScript program to find the maximum number in an array.***
```
  let myArray = [1,2,40,34,47,87,56,90,23]

function findMaxNumber(myArray){
  return Math.max(...myArray)
}
console.log(findMaxNumber(myArray))
```

***3)How to find duplicate elements in an array.***
```
const myArray = [1,2,1,1,3,2,4]

function duplicateArrays(item) {
  return item.filter(function(element, index){
    return item.indexOf(element) !== index;
  })
}
const duplicateElements = duplicateArrays(myArray)

console.log(duplicateElements)
```
