- The word ```implicit``` means: suggested though not directly expressed. (함축적인)
- It means when you don't provide a return, JavaScript will automatically return undefined for you.
- To sum up, if you forget to return from a function, the function will return undefined. 
(A quick reminder that the purpose of most functions is to return something. So don't forget to return from them the result that you've calculated.)

```
function getNameLength(name) {
    name.length
}
```
You have to learn to read the code above as if it was written like below:
```
function getNameLength(name) {
    name.length
    return undefined // implicit return added by JavaScript
}
```

## Branching
```
function canVote(age) {
    if (age >= 18) {
        return true
    }
}

console.log(canVote(30)) // This will return 'true'
console.log(canVote(10)) // This will return 'undefined'
```
If we apply what we learned from the previous lesson, we know that for all the other cases where age >= 18 will be ```false```, we do **NOT** have a return which means an implicit return will be added by JavaScript. So the final result will look like:
```
function canVote(age) {
    if (age >= 18) {
        return true
    }
    return undefined // implicit return added by JavaScript
}
```
So it's important to know that this will return ```undefined``` and not ```false``` (because there's no return false anywhere).
