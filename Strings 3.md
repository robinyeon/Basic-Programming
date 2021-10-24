## Multi-line strings
Sometimes you wish to create a string that spans multiple lines (a string that contains a newline character, which is the character generated when you press the Enter button on your keyboard). In JavaScript, this is only possible with a template string. For example:
```
let message = `Welcome to
our Website!`
```
Meaning that in JavaScript, you cannot have a multi-line string with a single quote or double quote strings.

## Can I always use template strings?
A common question that arises here is: Since template strings are more powerful, can I just always use them and avoid writing double quote or single quote strings?     
The answer is yes you can! There's no harm in doing that. However, from experience, it seems that people often fallback to double-quote strings for short strings mostly because we're used to it. But if you're new to programming and feel like you can always keep on writing template strings then that's perfectly fine.

## Escaping characters
```
let message = "Welcome to Sam's website" // works, no problem
```
```
// this WON'T work 👎
let message = 'Welcome to Sam's website'
```
- When you need to use ' or " as part of the string rather than the closing character, you need to escape it.
- You escape a character by prefixing it with a backslash. For example \' escape ' and \" escapes ".
```
// this works 👍
let message = 'Welcome to Sam\'s website'
```

- Using template strings
```
let message = `This is Sam's website and it's "awesome"!`

```


## Advanced Interpolation
```
function getWelcomeMessage(name) {
    return `Welcome ${name.toLowerCase()}`
}
```
```
function getMessage(age) {
    return `You are currently ${age} years old. Next year, you will be ${age + 1} years old.`
}
```
- You can interpolate expressions not just variables.







