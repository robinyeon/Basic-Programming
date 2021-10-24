## What is reduce?
- The ```reduce()``` method is to calculate a single value from an array.
- In other terms, the ```reduce()``` method reduces an array into a single value.
- The most common use cases of reduce (when working with arrays of numbers) are sum & multiplication.
- The ```reduce()``` method takes a reducer(callback) which allows you to configure the logic of how the array will be reduced into a single number.

## Array reduce: sum
```
let grades = [10, 15, 5]

let sum = grades.reduce(function(total, current) { 
    return total + current
}, 0);
```
- The ```reduce()``` method takes 2 parameters: ```reducer``` and ```initialValue```. ```.reduce(reducer, initialValue)```.
- The ```initialValue``` is always 0 for sum.
- The reducer is a callback function that receives 2 arguments: ```total``` and ```current```.
- The ```total``` (also called ```accumulator```) keeps track of the result of the reduce method. For example, when calculating the sum, it keeps track of the sum, step by step.
- The ```current``` represents one item of the array.
- The ```reducer``` is called for every item in the array.

## Array reduce: multiplication
For multiplication, we use an initialValue of 1.
```
let numbers = [5, 2, 10]

let result = numbers.reduce(function(total, current) {
    return total * current
}, 1)
```

## ```.forEach``` & ```.reduce```
### Using .forEach
```
let sum = 0
numbers.forEach(function(number) {
    sum = sum + number
})
```

### Using .reduce
```
let sum = numbers.reduce(function(total, current) {
    return total + current
}, 0)
```
- One of the similarities is that the initialValue was let sum = 0 but now it's the second argument passed to .reduce().
- One of the differences is that .forEach does not return anything whereas reduce returns a result (in this case the sum).
