#### CSV export ```arr.join([seperator])```
- CSV: comma-separated values
- 하나의 문자열로 변환
- 변환 후 엑셀에서 사용 가능
- seperator 생략시 기본적으로 "," 삽입
```
let arr = ['바람', '비', '물'];

console.log(arr.join());
// 바람,비,물

console.log(arr.join(''));
// 바람비물

console.log(arr.join('-'));
// 바람-비-물
```

---

#### ```string.startsWith(characters)```
It returns ```true``` when those characters are found **at the beginning** of the string and ```false``` otherwise.
```
let string = "Hello World!";

string.startsWith("H"); // true
string.startsWith("h"); // false
string.startsWith("Hello"); // true
string.startsWith("World"); // false
```
---
#### ```string.endsWith(characters)```
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
#### Procedural Programming(절차적 프로그래밍) vs Object Oriented Programming(객체지향 프로그래밍)
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

---
#### DRY "Don't Repeat Yourself!"

---
#### ```Number.parseInt(문자열 ,10)```
You can convert a string to a number as follows: ```Number.parseInt(stringValueHere, 10)```.

---
#### ```string.split(seperator)```
The ```.split()``` method will split the string based on the separator and **it will place every match in an array item**.
```
let days = "Monday;Tuesday;Wednesday;Thursday;Friday;Saturday;Sunday";

let array = days.split(";");
console.log(array); // ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday"]
```

---
#### HTML entities
To represent some symbols (such as the copyright symbol, the euro currency, etc.) on your page, you can use HTML entities.    

An HTML Entity is an instruction that displays such symbols and it looks like this:
```
&copy; // ©
&eur; // €
```
It starts with an ampersand (&) character and ends with a semi-colon (;).     

---
***Remember that it's not about memorizing those methods and/or getting the solution right from the first time. Rather it's about knowing how to resolve errors and finding the information (such as method names) whenever they're needed.***
