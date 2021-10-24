
```
function sumNonFreezingTemperatures(temperatures) {
    let sum = 0
    temperatures.forEach(function(temperature){
        if (temperature>0) {
            sum += temperature
        }
    })
    return sum
}
```
