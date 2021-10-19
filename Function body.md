## .trim()
The ```.trim()``` method allows us to make a new copy of the string while removing leading and trailing spaces from the original string.    
e.g.
```
"   alex   " to "alex"
```
```
let email = "   robin.yeon@gmail.com    "
email.trim()
```

----

```
function getEmail(email) {
    let cleaned = email
    cleaned = cleaned.toLowerCase()
    cleaned = cleaned.trim()
    return cleaned
}
```
1. Create a variable cleaned.   
2. Give it the value of: a copy of email but in lower case.   
3. Change the value of cleaned to a copy of its previous value but this time trimmed.  
 
cf. the reason why we lower case the email is because it's case insensitive, meaning that ```alex@gmail.com``` is the same email as ```ALEX@GMAIL.COM```. So to make sure that they are seen as the same by our website, we always lower case it.

## Re-assigning the variable
```cleaned = cleaned.trim()```
- changing the value of ```cleaned```.
- ```.trim()``` is **only creating a copy** of that variable, but for you to change ```cleaned```, you **have to re-assign** it to ```cleaned``` again.

***THIS IS WRONG(BELOW)***
```
function getEmail(email) {
    let cleaned = email
    cleaned.toLowerCase()
    cleaned.trim()
    return cleaned
}
```
- have to re-assign by writing ```cleaned=cleaned.toLowerCase()``` and ```cleaned=cleaned.trim()``` to be able to change the value of the ```cleaned``` variable..


## Add console.logs to visualize
To be able to visualize how these transformations are happening, feel free to add console logs.
```
function getEmail(email) {
    let cleaned = email
    console.log(cleaned) // will be the same as email
    cleaned = cleaned.toLowerCase()
    console.log(cleaned) // will be in lower case
    cleaned = cleaned.trim()
    console.log(cleaned) // will be without leading/trailing spaces
    return cleaned
}
```
- Make sure to keep the return cleaned at the end. Because the return will quit the function and return that value as a result.















