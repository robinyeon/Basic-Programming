```
let firstName = "Sam";
let lastName = "Blue";
let age = 30;

getFullName(firstName, lastName); // "Sam Blue"
getInitials(firstName, lastName); // "SB"
canVote(age); // true
```
Now compare above code to the code below, which assumes that we have a **class** called ```User``` defined somewhere
```
let sam = new User("Sam", "Blue", 30);
sam.getFullName(); // "Sam Blue"
sam.getInitials(); // "SB"
sam.canVote(); // true
```

## Why do we need classes?
A class allows us to group together all the variables and functions describing an entitiy in our application (for example a user, a person, an employee, a recipe, etc.).

### What about objects?
- So how is a class different than an object then?    
- An object is only a representation of variables, whereas a class also defines the behavior because we can have ```functions``` related to that entity.    
- For example, an object ```user``` will contain key/value pairs describing a user. Whereas a class ```User``` will contain variables and functions describing a user. (A class groups vairables and functions together.)    

## Methods & Properties
Once you start working with classes, the variables inside a class are called **properties** and the functions inside a class are called **methods**.

<br/>

***Classes are not only used for grouping variables and funcitons, in fact, there's a very important concept that is unique to classes, and that is 'instantiation(예시화)'.***
*instantiate: 구체적 예를들어 나타내다, 예시하다*

## Instantiation
```
let sam = new User("Sam", "Blue", 30);
sam.getFullName(); // "Sam Blue"
sam.getInitials(); // "SB"
sam.canVote(); // true

let charley = new User("Charley", "Don", 17);
charley.getFullName(); // "Charley Don"
charley.getInitials(); // "CD"
charley.canVote(); // false
```
- They are both **instantiated** (created) from the same ```class``` **User**, but they both have different properties (variables). Also, calling methods (functions) on these variables gives us different results depending on which variable we're calling it on.


## The 'new' keyword
Because ```User``` is a class, you can create a **new instance of that class** with the ```new``` keyword.

### What's an instance?

Output of ```console.log(sam)```(simplified):
```
User {
    firstName: "Sam",
    lastName: "Blue",
    age: 30,
    getFullName: function() {...},
    getInitials: function() {...},
    canVote: function() {...}
}
```
- You can see that the ```sam``` is an object.
- We can see the word **User** before that object in the console because this is not *any* kind of object, but it's a specific object.
- It's an object created by the ```User``` class.
- So the result of new User(...) will always be an object.
- **You create a new instance of a class, you will get back an object.**

## So what is a Class?
***A class is a factory that creates objects***
- A class is a **blueprint** for creating objects.
- The ```class User``` is the blueprint for creating user objects

## Sum up
- You can create a **new instance of a class** with the ```new``` keyword.
- When you create a new instance of a class, you will get back an object.
- A class is a factory that creates objects.
- A class is a **blueprint** for creating objects.




















