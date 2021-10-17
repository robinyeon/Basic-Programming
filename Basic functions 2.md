### Multiple parameters

when we have more than 1 parameter, you have to seperate them with a comma: ```function add(a, b)```.


```
function triple(number) {
  return number * 3
}

triple(5)
```
- the ```number``` variable is called a parameter
- the **5** that is passed to triple in ```triple(5)``` is called an argument.  
-> the argument 5 becomes the parameter for that function call.   
-> The argument is a value passed to a function. The argument becomes the parameter for that specific function call.    
-> 인수가 함수로 넘겨지고, 함수가 호출 됨으로써 파라미터로 변한다.   
(the argument 5 = 인수 5) (fuction call = 함수 호출)      


### Variable scope
***the parameter is only accessible inside the function, but nowhere else.***(this concept is called variable scope)
```
// number here is NOT defined
function double(number) {
  // number can only be used INSIDE this function
  return number * 2
}
// number here is NOT defined
```

### Store the result of a function
Since functions return a result, you can in fact store that result in a variable.     
e.g.  
```
function double(number) {
  return number * 2
}
let firstResult = double(4)
let secondResult = double(10)
```
- the result of ```double(4)``` into the variable ```firstResult```
- the result of ```double(10)``` into the variable ```secondResult```






