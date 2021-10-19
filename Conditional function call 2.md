e.g. 
```
function double(x) {
    return x * 2
}

function run(operation, x) {
    if (operation === "double") {
        return double()
    }
}

// Sample usage
run("double", 4) // doesn't work yet
run("double", 5) // doesn't work yet
```
The ```run``` function receives the parameter ```x```, which for example can be 4 or 5.   
We need to take that parameter and pass it to the double function. So instead of calling ```double()```, we need to call ```double(x)```.

```
function double(x) {
    return x * 2
}

function run(operation, x) {
    if (operation === "double") {
        return double(x) // take the x parameter and pass it to double
    }
}

// Sample usage
run("double", 4) // will return 8
run("double", 5) // will return 10

```
- You can pass a parameter from a function to another one.


