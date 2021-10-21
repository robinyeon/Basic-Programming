## If...else without else
```
function canVote(age) {
    if (age >= 18) {
        return true
    } else {
        return false
    }
}
```
the code above can be rewritten as following:
```
function canVote(age) {
    if (age >= 18) {
        return true
    }
    return false
}
``` 
These 2 code snippets work exactly the same.  
You can consider the above a bit of an "advanced" way to write the ```if...else```. 
