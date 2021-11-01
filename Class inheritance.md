```
// class definition
class Employee {
    constructor(firstName, lastName) {
        this.firstName = firstName;
        this.lastName = lastName;
    }

    getFullName() {
        return `${this.firstName} ${this.lastName}`;
    }

    getInitials() {
        return this.firstName[0] + this.lastName[0];
    }
}
```
```
// class definition
class Admin {
    constructor(firstName, lastName) {
        this.firstName = firstName;
        this.lastName = lastName;
    }

    getFullName() {
        return `${this.firstName} ${this.lastName}`;
    }

    getInitials() {
        return this.firstName[0] + this.lastName[0];
    }

    paySalaries() {
        console.log("Paying salaries...");
    }
}
```
- The ```constructor()```, ```getFullName()``` and ```getInitials()``` are exactly the same in both classes **Admin** and **Employee**.
- **DRY** means Don't Repeat Yourself.
- When you notice that several instance methods are being copy-pasted in different parts of your code, it generally means that you're violating the DRY principle.

## Extend parent
The class ```Admin``` and ```Employee``` share a lot of common functionality. So instead of writing these common methods in both classes, we only write them in the ```parent``` class. The ```parent``` class is the class that contains all the shared functionality.   
Then, the ```child``` class inherits all of these methods from the ```parent``` class.
```
// class definitions
class Employee {
    constructor(firstName, lastName) {
        this.firstName = firstName;
        this.lastName = lastName;
    }

    getFullName() {
        return `${this.firstName} ${this.lastName}`;
    }

    getInitials() {
        return this.firstName[0] + this.lastName[0];
    }
}

class Admin extends Employee {
    paySalaries() {
        console.log("Paying salaries...");
    }
}
```
- The ```child``` class (in this example, ```Admin```) will also inherit the ```constructor()```.

### Common mistake
***It's important to make sure that the ```parent``` class is defined first so that you are able to inherit from it in another class.***
incorrect:
```
// ❌ INCORRECT (Rectangle should be defined first)
class Square extends Rectangle {
    // ...
}

class Rectangle {
    // ...
}
```
correct:
```
// ✅ correct
class Rectangle {
    // ...
}

class Square extends Rectangle {
    // ...
}
```
- A ```child``` class can also access instance variables from its ```parent```.

## Overriding parent methods
- When a ```child``` class inherits from a ```parent``` class, all the instance methods are inherited. You can then decide to override some of them by re-defining them in the ```child``` class.






