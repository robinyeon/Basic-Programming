## Functions with array parameters
You may have noticed that all array names that we've used so far are in the **plural**. That's a very good habit to have. It's a best practice because arrays are made to contain more than 1 item. So having their name in plural will make it easier for you to reason about the array.

What would happen if you have the following array:
```
let grades = [10, 5, 12]
```
which contains 3 items, and you try to access ```grades[3]``` (corresponding to the 4th element) or ```grades[4]``` (corresponding to the 5th element)?
These elements don't exist, which is why you get back **undefined**.
