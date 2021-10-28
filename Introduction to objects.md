### Why do we need objects?
```
let firstName = "Sam";
let lastName = "Doe";
let age = 21;
let email = "sam@gmail.com";
let isVerified = true;
```
```
let person = {
    firstName: "Sam",
    lastName: "Doe",
    age: 21,
    email: "sam@gmail.com",
    isVerified: true
};
```
- This ```person``` object is a variable that represents one person. It contains the ```firstName```, ```lastName```, ```age```, ```email```, and ```isVerified``` of that person. These are called the **keys**. Every key has a value, for example, the ```firstName``` key has a value of **"Sam"**. The ```isVerified``` key has a value of **true**.
- Notice how objects are different than arrays because they have ```keys``` and ```values```. Whereas arrays only contained ```values``` (we previously defined arrays as being a list of values).

## Object
An object is a data type that allows you to group **several variables together into one variable** that contains keys and values.

## Objects syntax
an empty object:
```
let person = {}
let config = {}
```

Recommend you write the object on multiple lines like the example below:
```
let person = {
    firstName: "Sam"
};

let config = {
    units: "metric"
};
```

Always add a comma after every key/value pair (even the last one):
```
let person = {
    firstName: "Sam",
    lastName: "Doe",
};

let config = {
    units: "metric",
    currency: "USD",
};
```

## Read a key
Reading a specific key from an object in JavaScript follows the following syntax: ```objectName.keyName```  
So we use a **dot** (```.```) to access the key.
```
function getUserAge(user) {
    return `The user is ${user.age} years old`;
}

// Sample usage
let person = {
    name: "Sam",
    age: 20
};

getUserAge(person); // "The user is 20 years old"
```

## Update a value
```
let person = {
    name: "Sam",
    age: 20
};

person.age = 25;

console.log(person); // {name: "Sam", age: 25}
```
So we also use the **dot** to access a specific key (the ```age``` in this example) and then assign it to a new value with  ```= 25```.








