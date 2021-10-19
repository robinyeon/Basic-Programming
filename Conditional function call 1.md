## Conditional function call
```
function double() {
    console.log("Will double the number")
}

function run(operation) {
    if (operation === "double") {
        return double()
    }
}

// Sample usage
run("double")
```
- You can call functions inside if conditions.
- Calling functions inside if conditions allows your program to handle more complicated use cases.

### Code interpretation: top to bottom
### Code execution: follows the logic of your program
While code interpretation is happening top to bottom,   
the code execution is not necessarily top to bottom.
