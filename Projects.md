### CSV export ```.join(", ")```
---

### ```string.startsWith(characters)```
It returns ```true``` when those characters are found **at the beginning** of the string and ```false``` otherwise.
```
let string = "Hello World!";

string.startsWith("H"); // true
string.startsWith("h"); // false
string.startsWith("Hello"); // true
string.startsWith("World"); // false
```
---
### ```string.endsWith(characters)```
Returns ```true``` when the characters are found **at the end** of the string and ```false``` otherwise.
```
let string = "Hello World!";

string.endsWith("!"); // true
string.endsWith("d"); // false
string.endsWith("Hello"); // false
string.endsWith("World"); // false
string.endsWith("World!"); // true
```
---
### Procedural Programming(절차적 프로그래밍) vs Object Oriented Programming(객체지향 프로그래밍)
- Procedural programming: a list of instructions one by one.
```
let firstName = "Sam";
let lastName = "Blue";
let age = 30;

getFullName(firstName, lastName); // "Sam Blue"
getInitials(firstName, lastName); // "SB"
canVote(age); // true
```

- Object Oriented Programming(OOP): allows for better code reuse because you can create a new instance of a class and call the instance methods on it.
```
let user = new User("Sam", "Blue", 30);
user.getFullName(); // "Sam Blue"
user.getInitials(); // "SB"
user.canVote(); // true
```
--> the OOP one is cleaner and easier to read

