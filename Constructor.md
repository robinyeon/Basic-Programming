## Class constructor
```
// class definition
class User {
    constructor() {
        console.log("creating instance");
    }
}

// class usage
let user1 = new User(); // "creating instance" will be logged to the console
let user2 = new User(); // "creating instance" will be logged to the console
```
- We will use this ```constructor()``` method to set up the instances that we're creating. 

### Syntax
```
class User {
    constructor() {
        // code here will be automatically on every new instance creation
    }
}
```
- The ```constructor()``` method goes inside the class definition because **it's part of the class**.
- So functions defined inside a class (which are called methods), do not use the ```function``` keyword. They directly go inside the class and take the parentheses after their name and the curly braces.
  - The syntax of writing the ```constructor()``` is the name of the method, followed by parentheses and curly braces. No ```function``` keyword.

## Constructor parmeters
- Just like any function, the constructor method can accept parameters.
- The parameters for the constructor method are received when the instantiation of the class happens, meaning when you call ```new``` on the class.
```
// class definition
class User {
    constructor(firstName, lastName) {
        console.log("creating instance user");
        console.log(firstName)
        console.log(lastName);
    }
}

// class usage
let sam = new User("Sam", "Doe");
```
we will see the following logged to the console:
```
creating instance user
"Sam"
"Doe"
```















