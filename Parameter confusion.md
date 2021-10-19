## grade vs number
e.g.
```
function double(number) {
    return number * 2
}

let grade = 10
double(grade) 
```
- The variable ```grade``` has given the value ```10``` to the variable number, because ```number``` is a **parameter**. 
- However, this does NOT mean that the variables ```grade``` and ```number``` are the same!
- The variable ```number``` is ONLY defined inside the function ```double```. This is what we call **variable scope**.

## Parameter confusion
- The common confusion that happens with developers is when *you declare a variable with the same name as the parameter.*
- The ```parameter``` is only available inside the function.
- It may be confusing when the name of a ```variable``` is the same as a ```parameter``` but remember that they are NOT connected.
e.g.
```
function double(number) {
    return number * 2
}

let number = 10
double(number)
```
```let number = 10```is different than the ```number``` parameter inside the function.
