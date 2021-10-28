## Array as object value
```
let student = {
    firstName: "Sam", //string
    lastName: "Doe", // string
    hasGraduated: false, // boolean
    age: 21, // number
    grades: [15, 18, 14, 17], // array of numbers
    interests: ["computers", "books"] // array of strings
};
```
You can get the number of items in the array by accessing the ```.length``` property, you can iterate with ```.forEach()``` or transform the array into a new one with ```.map()```.    
For example: 
```
student.grades.forEach(function(grade) {
    console.log(grade);
});
```

## Nested objects
One useful feature of objects is that they can be **nested**!   
This means an object can contain (several) other objects.   
```
let student = {
    firstName: "Sam",
    lastName: "Doe",
    age: 21,
    currentCourse: {
        name: "Learn Programming",
        instructor: "Jad Joubran",
        isCompleted: false
    }
};

console.log(student.firstName); // "Sam"
console.log(student.currentCourse); // {name: "Learn Programming", instructor: "Jad Joubran", isCompleted: false}
```
We'd like to recommend that you use ```console.log()``` every step of the way so that you can visualize where you're at.


## Property vs Method
It is also possible for an object to contain a **function**. For example:
```
let user = {
    firstName: "Sam",
    lastName: "Doe",
    age: 21,
    canVote: function(age) {
        return age >= 18
    }
};
```
You can call that function by accessing the key ```canVote``` and then adding the parentheses afterward:
```
user.canVote(30); // true
```

- When the **key** has a value that is either a string, number, boolean, array, or object then it's called a **property**.      
- Whereas, when the **key** has a value that is a function (for example the canVote) then we say that it's a **method**.      
This is why you often see people referring to the ```firstName``` property, and the age property, and the ```canVote``` method.     
We've used the keyword **key** before, which is correct but ```property``` or ```method``` is more specific.

## Value as a variable
The value of a property can be a variable, for example:
```
let name = "Sam";

let user = {
    name: name,
    age: 21
};

console.log(user); // {name: "Sam", age: 21}
```
The object ends up containing the **value** of the variable which is, in this example, **"Sam"**.

***It's important to console.log() the object so that you can visualize it. This is NOT a tip for beginners. This is a tip for all developers, so don't be ashamed of using console.log ;)***


