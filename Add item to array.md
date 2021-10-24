Arrays are powerful data structures because they have several **methods** that you can call on them.      
(fyi) A method is a function that you can call on a certain data structure.   

## .push()
The ```.push(item)``` method adds (or pushes) an item into an existing array.
```
let numbers = []
console.log(numbers) // []

numbers.push(10)
console.log(numbers) // [10]

numbers.push(15)
console.log(numbers) // [10, 15]

numbers.push(13)
console.log(numbers) // [10, 15, 13]
```
- Notice how every time you call ```push(item)``` it adds that item at **at the end of the array.**
- You could start from an array that already contains items.

## What does ```.push()``` return?
The ```.push(item)``` method returns the new length of the array. So it returns a number.     
Let's take a look at what happens if we console.log the ```.push()``` calls:
```
let numbers = []

console.log(numbers.push(10)) // 1 (the new length of the array)
console.log(numbers) // [10]

console.log(numbers.push(15)) // 2 (the new length of the array)
console.log(numbers) // [10, 15]

console.log(numbers.push(13)) // 3 (the new length of the array)
console.log(numbers) // [10, 15, 13]
```
This means that if we assign the result of .push() into a variable, it will be a number representing the new length of the array:     
```
let numbers = [10, 20]

let value = numbers.push(15)
console.log(value) // 3 (new length of the array)
```

Most often, you will need to return the new array rather than the new length of the array, which is why you have to ```return``` the array after you ```.push()``` rather than returning the result of ```.push()```.
INCORRECT
```
function addTemperature(temperatures) {
    return temperatures.push(10)
}
```

CORRECT
```
function addTemperature(temperatures) {
    temperatures.push(10)
    return temperatures
}
```






