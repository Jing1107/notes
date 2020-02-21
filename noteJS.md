```
let listOfNumbers = [2, 3, 5, 7, 11];
console.log(listOfNumbers[2]);
// → 5
console.log(listOfNumbers[0]);
// → 2
console.log(listOfNumbers[2 - 1]);
// → 3

const property = 'name';
const hero = {
  name: 'Batman'
};

// Square brackets property accessor:
hero['name'];   // => 'Batman'
hero[property]; // => 'Batman'

let fruits = ['Apple', 'Banana']
fruits.forEach(function(item, index, array) {
  console.log(item, index)
})
```
1. Write a JavaScript function to check whether an `input` is an array or not.
-------------------------------------
Test Data :
console.log(is_array('w3resource'));
console.log(is_array([1, 2, 4, 0]));
false
true
```
var is_array = function(a) {
    return Array.isArray(a)
}
```
2. Write a JavaScript function to clone an array.
Test Data :
console.log(array_Clone([1, 2, 4, 0]));
console.log(array_Clone([1, 2, [4, 0]]));
[1, 2, 4, 0]
[1, 2, [4, 0]]
```
var array_Clone = function(a) {
    return a.slice(0)
}
```
3. Write a JavaScript function to get the first element of an array. Passing a parameter 'n' will return the first 'n' elements of the array.
Test Data :
console.log(first([7, 9, 0, -2]));
console.log(first([],3));
console.log(first([7, 9, 0, -2],3));
console.log(first([7, 9, 0, -2],6));
console.log(first([7, 9, 0, -2],-3));
Expected Output :
7
[]
[7, 9, 0]
[7, 9, 0, -2]
[] // cannot solve
```
var first = function(arr, n) {
    if(n==null) {
        return arr[0]
    };
    if(n<0) {
        return []
    }
    return arr.slice(0, n)
}
```
4. Write a JavaScript function to get the last element of an array. Passing a parameter 'n' will return the last 'n' elements of the array.
Test Data :
console.log(last([7, 9, 0, -2]));
console.log(last([7, 9, 0, -2],3));
console.log(last([7, 9, 0, -2],6));
Expected Output :
-2
[9, 0, -2]
[7, 9, 0, -2]
```
var last = function(arr, n) {
    if(n==null) {
        return arr.slice(-1)[0]
    };
    return arr.slice(-n)
}
```
5. Write a simple JavaScript program to join all elements of the following array into a string.
Sample array : myColor = ["Red", "Green", "White", "Black"];
Expected Output :
"Red,Green,White,Black"
"Red,Green,White,Black"
"Red+Green+White+Black"
```
myColor.toString()
myColor.join()
myColor.join('+')
```
6. Write a JavaScript program which accept a number as input and insert dashes (-) between each two even numbers. For example if you accept 025468 the output should be 0-254-6-8.

7. Write a JavaScript program to sort the items of an array. Go to the editor
Sample array : var arr1 = [ 3, 8, 7, 6, 5, -4, 3, 2, 1 ];
Sample Output : -4,-3,1,2,3,5,6,7,8
```
arr1.sort()
```
8. Write a JavaScript program to find the most frequent item of an array.
Sample array : var arr1=[3, 'a', 'a', 'a', 2, 3, 'a', 3, 'a', 2, 4, 9, 3];
Sample Output : a ( 5 times )
```
var arr1=[3, 'a', 'a', 'a', 2, 3, 'a', 3, 'a', 2, 4, 9, 3];

function findArr(array, times) {
    var count = 0;
    for (var i = 0; i < array.length; i++) {
        if(array[i]===times) {
            count++;
        }
    }
    return count;
}
findArr(arr1, 'a')+ ' ' +'times'
```
```
function countInArray(array, times) {
    return array.filter(item => item == times).length;
}
```
9. Write a JavaScript program which accept a string as input and swap the case of each character. For example if you input 'The Quick Brown Fox' the output should be 'tHE qUICK bROWN fOX'.
```
str='The Quick Brown Fox';
convert='';
for(var i = 0; i < str.length; i++) {
  c = str[i];
  if(c === c.toUpperCase()) {
    convert += c.toLowerCase();
  } else if(c === c.toLowerCase()) {
    convert += c.toUpperCase();
  } else {
    convert += c;
  }
}
```
10. Write a JavaScript program which prints the elements of the following array.
Note : Use nested for loops.
Sample array : var a = [[1, 2, 1, 24], [8, 11, 9, 4], [7, 0, 7, 27], [7, 4, 28, 14], [3, 10, 26, 7]];
```
Sample Output :
"row 0"
" 1"
" 2"
" 1"
" 24"
"row 1"
------
------
```
```
a.forEach(function (item, index) {
    console.log('row ' + index + ':' + ' ' + item)
})
```
11. Write a JavaScript program to find the sum of squares of a numeric vector. 
```
var sqrtSum = function(array) {
    let sum = 0,
        i = array.length
    while (i--)
        sum += Math.pow(array[i], 2)
        return sum;
}
sqrtSum([0,1,2,3,4])
```
###### why can't use loop to get square first then get sum
```
var originalArr = [1, 2, 3, 4, 5];
function multiplyByThree(arr) {
    var newArr = [];
    
    for(var i = 0; i < arr.length; i++) {
        newArr[i] += arr[i] * 3;
    }
    return newArr;
}
```
12. Write a JavaScript program to compute the sum and product of an array of integers.
```
function a(array) {
    var sum = 0,
        mulity = 1;
    for (var i = 0; i < array.length; i++) {
        sum += array[i];
        mulity *= array[i]
    }
    console.log('Sum : '+sum + ' Product :  ' +mulity);
}
a([1, 2, 3, 4, 5, 6])
```
13. Write a JavaScript program to add items in an blank array and display the items.
14. Write a JavaScript program to remove duplicate items from an array (ignore case sensitivity).
```
function removeDuplicates(array) {
  return array.filter((a, b) => array.indexOf(a) === b)
}
```
15. We have the following arrays :
color = ["Blue ", "Green", "Red", "Orange", "Violet", "Indigo", "Yellow "];
o = ["th","st","nd","rd"]
Write a JavaScript program to display the colors in the following way :
"1st choice is Blue ."
"2nd choice is Green."
"3rd choice is Red."
##### Note : Use ordinal numbers to tell their position.

16. Find the leap years in a given range of years.
