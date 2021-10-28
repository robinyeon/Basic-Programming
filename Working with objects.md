## Adding a new key/value pair
1. ```obj.newKey = "newValue"```
```
let user = {
    firstName: "Sam",
    lastName: "Doe"
};

user.age = 20;
console.log(user); // {firstName: "Sam", lastName: "Doe", age: 20}
```

2. It is also possible to start from an empty object and add key/value pairs one by one. For example:
```
let config = {};

config.currency = "EUR";
config.theme = "dark";
console.log(config); // {currency: "EUR", theme: "dark"}

```
