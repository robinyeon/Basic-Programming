## JSDoc comments
```
/**
 * @param {array} grades
 */
```
This is a special comment that is only there to improve your programming experience in the text editor.   
It instructs the editor that the variable or parameter grades is an array. This will allow the text editor to provide you with auto-complete specific to arrays, thus relevant to you.

## Array.length
- We've got the ```.length``` property on arrays which returns **the number of items** in that array.
- The ```.length``` is a property, meaning that it's a value that has already been computed. It's NOT a function which is why you should not put the ```()``` afterward.

## Last item
The **number of items - 1** can be written as the following expression, assuming a variable called items: ```item.length-1```
```
let items = [10, 20, 30]

items[items.length - 1] // 30 (last item)
```
