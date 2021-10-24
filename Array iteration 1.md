## array.forEach()
- The .forEach() method allows us to iterate over an array.
- What the forEach does is that it allows you to run a function for every item of an array.
```
let grades = [14, 10, 18]

grades.forEach(function logGrade(grade) {
    console.log(grade)
})
```
1. Take the first item of the array, which is 14, and run the function ```logGrad```e while passing it the number 14.
2. Then it'll take the second item of the array, which is 10, and run the function ```logGrade``` while passing it the number 10.
3. And the same for the last item of the array, which is 18.

So the above code, translated into:
```
// You DON'T write this code, but this is what happens
logGrade(14)
logGrade(10)
logGrade(18)
```


## Callback
When calling functions, we've been used to calling them with a number, a string or a boolean.     
For example: ```canVote(20)```. We passed to the ```canVote``` an argument which is 20 and that is a number.    

However, you may have noticed, that with the .forEach(), we passed a function.    
We call this function a **callback** because this function is being called back automatically by the JavaScript.    
So what is a callback? A callback function is a function that is passed as an argument and that will be called by the programming language (sometimes at a later stage).

## Dropping the function name
When writing the callback for the ```.forEach``` method, you can actually remove the function name completely, that's because this function won't be re-used anywhere else, so it's meaningless to give it a name.      
So the below code:
```
let grades = [14, 10, 18]

grades.forEach(function logGrade(grade) {
    console.log(grade)
})
```
can be re-written by dropping the function name:
```
let grades = [14, 10, 18]

grades.forEach(function (grade) {
    console.log(grade)
})
```
We do recommend that you drop the function name. When you drop the function name, it's often referred to as **anonymous function**, which is a function without a name.     

