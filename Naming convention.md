## Cannot re-define a variable
We cannot re-define or re-declare ```name``` again because it has already been defined.   
***So after the first time you use ```let``` for a specific variable name, you cannot use it again.***    

*Below is INVALID. It will break with an ERROR*
```
let name = "Sam"
let name = "Alex"
```

If you want to make the code above valid, you can then drop the let keyword from the 2nd time you use the variable name:

*This is valid because we are not re-defining. We're just ***changing the value.****
```
let name = "Sam"
name = "Alex"
```

## Variables/Functions are case sensitive
-> Thus make sure to use the variable and function names exactly how you define them.   
- **case sensitivity**: "sam" and "SAM" are NOT the same.
- **case insensitivity**: "sam" and "SAM" are considered the same.    


## Cannot use a variable before declaring it
e.g. the code below will NOT work:
```
console.log(name) // this will break with an ERROR
let name = "Alex"
```
We should have defined the variable first and then console.log it.

## JavaScript naming convention_lowerCamelCase
The first character of the first word is in lower case, then the first character of the remaining words is in upper case.     
(Recommendations making it easier for other people to understand your code) 

## Boolean pro tip
When defining a variable that will contain a boolean value or a function that will return a boolean value, it's a good idea to give it a name that starts with ```can``` or ```has``` or ```is```.      
e.g. canVote, isLegal, hasVoted, isRegistered.



## Variable name
- you cannot start a variable name with a number.
- (Rather than knowing the exact rules for what a valid variable/function name is,)   
It's easier to always start it with a letter (any letter from a to z) or an _ (underscore).







