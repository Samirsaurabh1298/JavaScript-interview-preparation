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

***This is another approach*** 

function findDupEle(item){
   return item.filter(function(element,index){
   return item.indexOf(element, index + 1) !== -1;
})
}
const result = findDupEle(myArray)
console.log(result)
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


   *** Using find method ***

   function findcity(peopleArray, cityName){
      let filteredCity = peopleArray.find(function(item){
        return item.city === cityName;
      })
      return filteredCity
   }
   console.log(findcity(peopleArray, "bangalore"))
```

***6)How to find missing number in  given integer array of 1 to 10***

``` js
const arrNumber = [1, 2, 3, 4, 5, 6, 9, 10]

const findMissingNum = [];
const missingValue = (arr) => {
    const minValue = Math.min(...arr);
    const maxValue = Math.max(...arr)
    for (let i = minValue; i < maxValue; i++) {
        if (arr.indexOf(i) < 0) {
            findMissingNum.push(i)
        }
    }
    return (findMissingNum)
}

console.log(missingValue(arrNumber))
``` 

***7)How to find Even number in a array***

``` js
const myArrays = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
  const evenNumber = myArrays.filter(function(item){
      return item % 2 === 0;
  })
  console.log(evenNumber)
```


***8)How to find Odd number in a array***

``` js
const myArrays = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
  const oddNumber = myArrays.filter(function(item){
      return item % 2 == !0;
  })
  console.log(oddNumber)

```


***8)How to find sum of all elements in a given array in javascript.***

``` js
const myArray = [1, 2, 3, 5, 8, 9]

const sumOfNumber = (item) => {
   return item.reduce((prev, curr) => {
    return prev + curr
   })
}
console.log(sumOfNumber(myArray)).
```

***we can do by multiple way***

```js

function sumOfArr(item) {
  let sum = 0
    for(let i = 0; i < item.length; i++){
       sum += item[i]
    }
    return sum
}
console.log(sumOfArr(myArray))
```

***9)Write a function that returns an array of unique elements from the input array while preserving their original order.***

```js
const myArray = [1, 2, 3, 4, 1, 2, 5];
function findUniqueEle(item){
   const uniqueSet = new Set(item)
   return Array.from(uniqueSet)
}
const result = findUniqueEle(myArray)
console.log(myArray)
```
***10)Write a function that takes a string as input and returns the count of each character in the string as an object.***

```js
let charact = "hello";

function countOfChar(str) {
    let charCount = {};
    for (let i = 0; i < str.length; i++) {
        let char = str[i];

        if (charCount[char] === undefined) {
            charCount[char] = 1;
        } else {
            charCount[char]++;
        }
    }
    return charCount;  
}

console.log(countOfChar(charact));

```

***11)Write a function that takes an array of integers as input and returns the sum of all the positive integers in the array.***

```js

let myArray = [1, -2, 3, -4, 5];

function sumOfPositive(item) {
    return item.reduce(function(sum, num) {
        if (num > 0) {
            return sum + num;
        } else {
            return sum;
        }
    }, 0);
}

const result = sumOfPositive(myArray);
console.log(result); // Output: 9
```
***12)string is reversed.***

```js
let name = "Asynchronous"
function reversedStr(name){
  let reversed = "";
for(let i = name.length -1; i >= name; i--){
reversed+= name[i]
}
return reversed
}

console.log(reversedStr(reversed))
```

***13)Write a function that takes this array of student objects as input and returns an array of names of students who are in grade "A" .***

```js
const students = [
    { name: "Alice", age: 20, grade: "A" },
    { name: "Bob", age: 21, grade: "B" },
    { name: "Charlie", age: 22, grade: "A" },
    { name: "David", age: 23, grade: "C" }
];

const getGradeAStudents = students
    .filter(function(student) {
        return student.grade === "A";
    })
    .map(function(student) {
        return student.name;
    });

console.log(getGradeAStudents); // Output: ["Alice", "Charlie"]

```
***14)How to log all pairs of Arrays?***
```js
const boxes = [1, 2, 3, 4, 5, 6]

function logAllPairsOfArrays(item){
  for(let i = 0; i < item.length; i++){
    for(let j = 0; j < item.length; j++){
      console.log(item[i], item[j])
    }
  }
}
logAllPairsOfArrays((boxes))

function logAllPairsOfArrays(item){
  item.forEach(function(firstBox){
    item.forEach(function(secondBox){
      console.log(firstBox, secondBox)
    })
  })
}

logAllPairsOfArrays(boxes)
```

***14)Write a function that reverse a string LIKE- "Hi my name is Samir", should be like this => "rimaS si eman ym iH. ***
```js
let originalString = "Hi my name is Samir"

function reverseString(str){
  let splitString = str.split("");
  let reverseArray = splitString.reverse();
  let reversedString = reverseArray.join("");
  return reversedString;
}

let reversedString = reverseString(originalString)
console.log(reversedString)

we can do it via multiple ways:-------

1) Using BUILT-IN Methods (split, reverse, join)
  function reverse2(str){
  return str.split('').reverse().join('')
}

let reversedStr = reverse2(originalString)
console.log(reversedStr)

2)Using SPREAD OPERATOR
  function spread3(str){
    return [...str].reverse().join("")
  }
  let reversedStr = reverse2(originalString)
console.log(reversedStr)
```
