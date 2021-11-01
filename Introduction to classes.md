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
