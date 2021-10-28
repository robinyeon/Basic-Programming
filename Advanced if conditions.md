#### Q.
Complete the function by returning true when the temperature is between 10 and 15 (inclusive) and false otherwise.  
After you complete the challenge, try to solve it without using an if/else condition (check the hints for an extra tip).    

#### A.
1. using an if/else condition
```
function isReady(temperature) {
    if (temperature >= 10 && temperature <= 15) {
      return true
    } else {
      return false
    }      
}
```
2. without using an if/else condition
```
function isReady(temperature) {
    return temperature >= 10 && temperature <= 15
}
```

