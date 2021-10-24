## Reading an item from the array
1. To access an item from an array, there's a new syntax for it which is the square brackets ```[]```
2. Inside the square brackets you should have the position of the item that you want to read. So for example ```[1]```
3. This syntax needs to go directly after the name of the array. So for the above example, it would look like ```grades[1]```
4. This is the tricky part. **The position starts at 0** (the index is 0-based).
```
let grades = [5, 3, 8]
grades[1] // 3
```

A quick note that we've been using the word position, but a more correct word that you will see people use would be **index**.  
So from now on, we'll start referring to the position as the **index** or **array index**.
