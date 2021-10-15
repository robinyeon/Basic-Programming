**A function is a reusable piece of code that performs some logic and gives you a result**

## Benefits of functions: resuability
example of a function
```
function double(number) {
  return number * 2
}
```

- ```number``` is a variable. In fact, ```number``` is a special kind of variable called a **parameter**, will discuss that later on.

1. The ```function``` keyword
The function keyword is used to define a function. This allows you to group related code logic together to make a reusable task.

2. The parentheses ```()```

3. The curly braces ```{}```

4. The ```return``` keyword
- The return keyword is used to give the *result* of the function.  
- By having ```return number *2``` you're saying that the result of the **double** function is: number * 2.
- The return keyword can only be used **inside** a function.


## Parameters
***A parameter is a variable that a function receives.*** 
With a different parameter and a different output.  
the ```number``` variable(in the above example) could have any value, it all depends on the value you provide when you call the function.

## Calling functions
```
function double(number) {
    return number * 2
}

double(5)
```
You are invoking the function doulbe and passing the value 5 to the ```number``` parameter.
-> So to call a function, you have to write its name(```double```) and then you need to have the parentheses```()``` with a value that
you want to pass for the parameter. Hence why it looks like: ```double(5)``` or ```double(20)```
