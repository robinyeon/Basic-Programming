```
let grades = [5, 3, 8]
```
But the first grade (5) needs to be changed to 6, here's how you can do that:
1. Ask yourself: how can I *read* that item that I want to change?
```grades[0] // returns 5```
2. Now assign it to the new value with the equal sign (```=```) and the new value like so:
```grades[0] = 6```
Full example:
```
let grades = [5, 3, 8]
grades[0] = 6
console.log(grades) // [6, 3, 8]
```

## Example with functions
CORRECT
```
function fixGrade(grades) {
    grades[0] = 6
    return grades
}
```

INCORRECT
```
function fixGrade(grades) {
    // this is INCORRECT
    return grades[0] = 6
}
```

## ```temperatures[0] = temperatures[0] + 1```
Here's how you should read it in plain English:     
The **new value of temperatures[0]** is equal to: the **current value** of ```temperatures[0]``` + 1.

