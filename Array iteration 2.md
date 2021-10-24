## forEach syntax
- In array iteration, try to distinguish between:
1. The ```.forEach()``` function call.
2. The function passed to the forEach.

- Always use the plural for the array and singular for the array item.
1. Make sure your array name is plural.
2. And make sure the function you pass to the forEach has the parameter in the singular.

- Always log the array item: It's a good idea to always have that ```console.log()``` first thing as it helps you visualize the shift from array to array item.

## Sum up
You can think of writing array iterations as 3 steps. Here's an example assuming the array grades
1. Start by writing ```grades.forEach()```
2. Then inside the forEach(), you need to write the function that will be called for every grade: ```function(grade) { }```
3. And finally, you add the ```console.log(grade)``` inside of that function.
Putting it all together, you get:
```
grades.forEach(function(grade) {
    console.log(grade)
})
```
