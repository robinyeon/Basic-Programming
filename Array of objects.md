## Array of objects
Arrays of objects are the most common data type because they allow us to represent a list of entities from the real world.  
```
let users = [
  {
    firstName: "Sam",
    lastName: "Blue",
    age: 21,
  },
  {
    firstName: "Charlie",
    lastName: "Bon",
    age: 38,
  },
  {
    firstName: "Okaley",
    lastName: "Drijf",
    age: 24,
  }
];

console.log(users[0].firstName); // "Sam"
```

## Working with arrays of objects
[array]는 index```[0]```로 접근하고, {object}는 **dot syntax**```.```으로 접근하자   

## Visualize the object
It's even more important here to console.log the object so that you can visualize it. This will make it easier for you to find the code that you're looking for.

## Common mistake
The most common mistake when it comes to arrays of objects, is trying to access a certain property on the array rather than on the object. For example:
```
let users = [
  {
    firstName: "Sam",
    lastName: "Blue",
    age: 21,
  },
  {
    firstName: "Charlie",
    lastName: "Bon",
    age: 38,
  }
];

// this is INCORRECT ❌
console.log(users.firstName); // undefined

// these are correct ✅
console.log(users[0].firstName);
console.log(users[1].firstName);
```
We can't access ```users.firstName``` because ```users``` is an array, thus it does not have a property ```firstName```.  
The ```firstName``` property is only available on the objects inside the array.

## Iterating over them ```.forEach()```

## Transforming with ```.map()```
```
let recipes = [
  {
    title: "Pasta pesto",
    preparationMinutes: 30,
    rating: 4.5
  },
  {
    title: "Lasagna",
    preparationMinutes: 45,
    rating: 3.9
  }
];
```
and we'd like to create an array of all the recipes names.    
The end result will look like this: ```["Pasta pesto", "Lasagna"]```.     
This is a **transformation** where we transform every **object** from the array into a **string**, which is the title of the recipe.
```
let titles = recipes.map(function(recipe) {
    console.log(recipe); // helps us visualize
    return recipe.title;
});
console.log(titles); // ["Pasta pesto", "Lasagna"]
```








