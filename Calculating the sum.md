## The hidden step
There's a hidden step in the calculation we made above, which is before we add the first item, **the sum was 0**.

So once we're going to write the code that sums an array, we need to tell the programming language that **we want to have a variable that will hold the sum.** But then, we need to give it a certain value. What would that be? 0? 1?

Because it's a sum, we start at 0.

So coming back to this array: ```[10, 5, 10]```.

1. We start by saying the ```sum``` is 0. ```let sum = 0```
2. Then we add the first item, which is 10. So far the sum is 10.
3. Then we add the second item, which is 5. So far the sum is 15.
4. Then we add the third item, which is 10. So far the sum is 25. The final sum is 25.

## Example without iteration
```
let grades = [10, 18, 14, 15]

let sum = 0

sum = sum + grades[0]
sum = sum + grades[1]
sum = sum + grades[2]
sum = sum + grades[3]
```

## Sum with array iteration
```
let grades = [10, 18, 14, 15]

let sum = 0
grades.forEach(function(grade) {
    sum = sum + grade
})
console.log(sum) // 57
```

## Common mistake
A common mistake is placing ```let sum = 0``` inside the ```function(grade) { ... }``` however, that will end up breaking your sum calculation because you are resetting the sum back to 0 for every item in the array
So make sure that you define the ```let sum = 0``` before the ```.forEach()```.

## ```+=```
The ```sum = sum + grade``` piece of code can be re-written as: ```sum += grade```.   
The ```+=``` operator means that it will take the old value and add to it.
