let listOfNumbers = [2, 3, 5, 7, 11];
console.log(listOfNumbers[2]);
// → 5
console.log(listOfNumbers[0]);
// → 2
console.log(listOfNumbers[2 - 1]);
// → 3



let fruits = ['Apple', 'Banana']
fruits.forEach(function(item, index, array) {
  console.log(item, index)
})

. Write a JavaScript function to check whether an `input` is an array or not. Go to the editor
Test Data :
console.log(is_array('w3resource'));
console.log(is_array([1, 2, 4, 0]));
false
true

var is_array = function(a) {
    return Array.isArray(a)
}
