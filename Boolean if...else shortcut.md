```
function canVote(age) {
    if (age >= 18) {
        return true
    } else {
        return false
    }
}
```
the above code can be re-written with a shortcut, completely removing the ```if...else```:
```
function canVote(age) {
    return age >= 18
}
```
If you were returning a string or a number, this pattern cannot be used.
