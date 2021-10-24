## Array.map()
Whenever you encounter these scenarios, where you need to transform an existing array into a new one, you should use the ```.map()``` method.   

The ```.map()``` method allows you to apply a transformation for every item in an array. Thus the end result will be an array containing the same number of items (but most likely different values for those items).

```
let grades = [10, 15, 13]

let doubledGrades = grades.map(function(grade) {
    return grade * 2
})
console.log(doubledGrades) // [20, 30, 26]
```

## Common Mistakes
- The most common mistake when it comes to .map() is forgetting the return keyword. 
- Mixing up forEach and map:
  + Another common mistake is mixing up ```.forEach``` and ```.map()```. The syntax is similar, and the concept of array iteration is also the same.
  + But the main difference is that ```.forEach()``` does NOT return anything. Even if you place a ```return``` inside it, you won't get a new array from the ``.forEach()```.
  + Thus use the ```.forEach()``` when you plan on iterating and ```.map()``` when you plan on transforming the array into a new one.
