***1)Write a JavaScript function to calculate the sum of two numbers.*** 
``` js
  function calculateTwoNum(a,b) {
    return a + b;
  }
  console.log(calculateTwoNum(2,3))
```

***2)Write a JavaScript program to find the maximum number in an array.***
``` js
  let myArray = [1,2,40,34,47,87,56,90,23]

function findMaxNumber(myArray){
  return Math.max(...myArray)
}
console.log(findMaxNumber(myArray))
```

***3)How to find duplicate elements in an array.***
``` js
const myArray = [1,2,1,1,3,2,4]

function duplicateArrays(item) {
  return item.filter(function(element, index){
    return item.indexOf(element) !== index;
  })
}
const duplicateElements = duplicateArrays(myArray)

console.log(duplicateElements)
```


***4)How to find min value of an array.***
``` js
let myArryNumber = [1, 9, 88, 68, 755]
  const minFunction = (arr) => {
      return arr.reduce(function(prev, curr){
        return prev < curr ? prev : curr
      })
  }
console.log(minFunction(myArryNumber))
```

***5)How to find Second largest value, and remove first largest value in an array.***

``` js
const numArray = [2,6,8,15,9]

function maxValue(numArray){
  firstLargestValue = Math.max(...numArray)
  index = numArray.indexOf(firstLargestValue)
  numArray.splice(index,1)
   secondLargestValue = Math.max(...numArray)
  return (secondLargestValue)
}
console.log(maxValue(numArray))
```

***6)How to to use find and filter method in given array of object.***
``` js
const peopleArray = [
    { name: "John", age: 25, city: "New York" },
    { name: "Alice", age: 30, city: "Los Angeles" },
    { name: "Bob", age: 22, city: "Chicago" },
    { name: "Eva", age: 28, city: "San Francisco" },
    { name: "Mike", age: 35, city: "Seattle" }
    { name: "Jo", age: 28, city: "New York" },
];

***How to to find age should be less than 30 in given array of object?***
   
   const filterAge = peopleArray.filter(function(item){
    return item.age > 30
   })
   console.log(filterAge)


   ***How to to find repeated city in given array of object?***

   function filtercity(peopleArray, cityName){
      let filteredCity = peopleArray.filter(function(item){
        return item.city === cityName;
      })
      return filteredCity
   }
   console.log(filtercity(peopleArray, "New York"))
```