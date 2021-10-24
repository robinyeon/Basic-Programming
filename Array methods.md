## ```.includes(item)```
- ```array.includes(item)``` allows you to check whether the item exists inside the array.
- ```array.includes(item)``` returns a boolean.
- ```array.includes(item)``` returns true when the item is found inside the array.
- ```array.includes(item)``` returns false when the item is NOT found inside the array.

Most of the times, ```numbers.include is not a function``` is caused by one of 2 issues:
1. Either numbers is not an array (thus you can't call array methods on it)
2. Or most commonly, you've made a typo in the method name.

## ```.join(glue)```
- The ```array.join(glue)``` method **converts the array into a string** by gluing together the items with the glue that you provide.
```
let numbers = [3, 1, 6]

let string = numbers.join(";") // "3;1;6"
```

Another common example is converting an array into CSV format:
```
let numbers = [3, 1, 6]
let csv = numbers.join(", ") // "3, 1, 6"
```
- CSV stands for Comma Separated Values and is a popular format as it can be easily imported into Excel.
- Notice how the glue in this example is: ```", "``` (that's a comma character followed by a space character).
- Without the space character, ```numbers.join(",")``` would end up converting the array into the following string: ```"3,1,6"```.

