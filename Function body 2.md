It's better to write your logic line by line, step by step rather than trying to cram it all on one line. This applies also for experts not just beginners.         
e.g.    
```
function getCoursePriceInCents(dollars) {
    return dollars * 100 + 200
}
```
```
function getCoursePriceInCents(dollars) {
    let amount = dollars * 100
    amount = amount + 200
    return amount
}
```

