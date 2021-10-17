### console.log()
As you start to work more with variables and functions, it becomes hard to remember what the value of some variable is, so it would be nice to have a way to visualize that.
- ```console.log()``` allows you to visualize your code in the console.
- the console is only visible to devolopers, but not the end-users(actual users).
- ```console.log()``` helps you find bugs(which is called: debugging).

### console.log & functions
```console.log``` works in functions too.     
<br/>
e.g.    
```
function double(number) {
  console.log(number * 2)
  return number * 2
}
```
- how even though we have a console.log, **we need to have the return** in the funciton.
- that's because ```console.log``` does NOT replace return.
- ```console.log``` will never modify the result of a function, it will just show you a string or a number in the console.
<br/>
Notice console.log can take a variable or even a function call and will print its result in the Console.    
e.g.  
```
function sum(a, b){
  return a + b
}

console.log(sum(3, 5))
```


### return "quits" the function
- when you have a ```return``` in your function, this will be the last line of code executed in that function.
- this means if you have a ```console.log``` on the line after the ```return```, it will not be executed. Thus you will not see its result.     
<br/>
e.g. (This function WORKS but we don't see the console.log) 
```
function double(number) {
  return number * 2 
  console.log(number * 2)
}
let result = double(4)
```
