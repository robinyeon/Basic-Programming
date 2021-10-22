interpolation: 써넣음, 내삽법

## Template strings
- Backtick character ``` ` ```
- Strings defined with the backtick character are called template strings.
- We call it a template string (but you can still call it a string) because it has additional capabilities such as interpolation.

## Interpolation
```
let name = "Alex"

let message = `Hello ${name}` // `Hello Alex`
```
We could have achieved the same result using concatenation, but the syntax is a bit more complicated for concatenation. 
It would have been: ```let message = "Hello " + name```, especially with regards to getting the space character correctly.  
So this is an interpolation, we inserted the variable ```name``` into the string ```Hello ```.


To write interpolation correctly, remember that interpolation requires 2 steps:
1. The string has to be a template string (which means, written using the backtick character). It does NOT work with string created with the double-quotes.
2. Wrap the variable with ```${``` and then ```}```.

## Concatenation vs interpolation
- You can use whichever one you prefer.
- You may be confused about how come it's possible to achieve the same task in multiple ways, but in fact, this is very common in programming. Often the same task can be achieved in several ways.
