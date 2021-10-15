## let is only for assignment
The **first time** you define a varable, you have to define it with ```let```,  
however the next time you **use** that variable, you should NOT use ```let``` anymore. 
```
let year = 2020
year = 2030
```
```
let year = 2020
let next = year + 1
```
-> We only used ```let``` **once** per variable declaration.    
-> So the second line of code had a let because we are defining a new varaible **next**.  

*The next time you use that variable, you should NOT use let any more. Just directly use the variable by its name.*


## Be careful of hardcoding
```
year = 2020, next = 2021  
year = 2100, next = 2100  
```
This is why you should not write ```let next = 2021```
-> **Hardcoding**: fixing the value which will then not change later on.

## Addition & multiplication
