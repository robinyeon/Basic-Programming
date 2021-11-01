## Instance variables
An instance variable is a variable that belongs to a specific instance of a class.    
There are two main benefits for creating instance variables:    
1. The instance variables you create in the constructor() method get returned as key/value pairs in the object returned by the constructor.
2. Most importantly, these instance variables can be used in **all instance methods** in the class. This topic is covered in the next chapter.
```
// class definition
class User {
    constructor() {
        // hardcoded examples for now
        this.firstName = "Sam";
        this.age = 24;
    }
}

// class usage
let user = new User();
console.log(user); // User {firstName: "Sam", age: 24}

```

### Why not define a variable with ```let```?
You might be wondering why did we define this ```age``` variable with ```this.age``` rather than ```let age = 30```.      
If you define the variable with ```let age = 30``` then it's **NOT** an instance variable anymore.      
It's just a variable that is **only** available in the constructor(). It will NOT affect the returned object and it will not be accessible anywhere else in the instance methods of this class.

## What is 'this'?
- The keyword ```this``` refers to the **current instance** of the class.
- ```this.X``` creates an instance variable **X**.
- Then every야 new instance of a class will contain an instance variable.

## Capture constructor params
```
// class definition
class User {
    constructor(firstName, lastName) {
        this.firstName = firstName;
        this.lastName = lastName;
    }
}

```
- ```this.firstName``` and ```firstName``` (and the same for ```this.lastName``` and ```lastName```).
- ```this.firstName``` is a new **instance variable** where as ```firstName``` is a constructor parameter.

```
// class usage
let sam = new User("Sam", "Blue");
console.log(sam); // {firstName: "Sam", lastName: "Blue"}
```
- Notice how we captured the parameters that we passed to the constructor (```"Sam"``` and ```"Blue"```) and we created 2 instance variables: ```this.firstName``` and ```this.lastName```.

## Recap_visualize
```
class User {
    constructor(age) {
        this.age = age;
    }
}

let sam = new User(20);
```
![visualized_Class](https://res.cloudinary.com/dbfn5lnvx/image/upload/w_1000/v1610195070/learnprogramming/lessons/instances.png)
