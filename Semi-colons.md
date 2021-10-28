## JavaScript and semi-colons
- JavaScript has semi-colons because it's common to minify the code before publishing the website.
- Automated tools will minify your code. You should never minify it yourself or write minified code.
- Minification works by removing the comments and removing all the white-spaces (thus putting all your code on 1 line). 


**Minification**
```
export function exportLowerCasedCSV(items) {
    return items.map(function(item) {
        return item.toLowerCase()
    }).join(", ")
}
```
switch above code into the below code:
```
export function exportLowerCasedCSV(items) {return items.map(function(item) {return item.toLowerCase();}).join(", ");}
```

## Using semi-colons: At the end of a statement
A statement is a piece of code that performs a very specific operation.
```
// variable declaration
let year = 2020;

// assigning a new value to a variable
year = year + 1;

// calling a function
console.log(year);
```
