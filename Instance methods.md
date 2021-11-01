## Instance methods
An instance method is a method that can be called on an instance of a class.
```
// class definition
class User {
    constructor(firstName, lastName) {
        this.firstName = firstName;
        this.lastName = lastName;
    }

    getFullName() {
        // TODO: we still have to properly implement the method here.
        // We will do that in the next lesson
        return "full name here";
    }
}
// class usage
let user = new User("Sam", "Doe");
user.getFullName(); // "full name here"
```
- Notice how ```.getFullName()``` is a method that we called on the ```user``` which is an instance of the class ```User```.

### Why are they useful?
moving from:
```
let firstName = "Sam";
let lastName = "Blue";
let age = 30;

getFullName(firstName, lastName); // "Sam Blue"
getInitials(firstName, lastName); // "SB"
canVote(age); // true
```
to:
```
let sam = new User("Sam", "Blue", 30);
sam.getFullName(); // "Sam Blue"
sam.getInitials(); // "SB"
sam.canVote(); // true
```
- We use instance methods to group together functionality based on its logic.
- For example, payment functions are defined in a class Payment as instance methods.
- The syntax of an instance method is similar to that of a constructor method.
```
class Payment {
    constructor(paymentMethod) {
        this.paymentMethod = paymentMethod;
    }

    canPay() {
        //code for canPay
    }

    hasPaid() {
        // code for hasPaid
    }

    redirectToBank() {
        // code for redirectToBank
    }
}
```

## Implementing instance methods
```
// class definition
class User {
    constructor(firstName, lastName) {
        this.firstName = firstName;
        this.lastName = lastName;
    }

    getFullName() {
        return `${this.firstName} ${this.lastName}`;
    }
}

// class usage
let user = new User("Sam", "Doe");
user.getFullName(); // "Sam Doe"
```
```
class User {
    constructor(firstName, lastName) {
        this.firstName = firstName;
        this.lastName = lastName;
    }

    getFullName() {
        // ❌ this is INCORRECT
        return `${firstName} ${lastName}`;
    }
}
```
- The parameters you receive in the constructor are NOT accessible in instance methods (because they are different methods, and parameters are only accessible in its own method).
- This is why we capture constructor parameters as instance variables which will allow us to use these instance variables in any instance method.
- A common mistake is attempting to use the variable name (that the constructor() receives) rather than the instance variable. So don't forget the ```this.``` syntax.


