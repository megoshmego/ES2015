Let's evaluate the important terms, ideas, and provide code snippets for each of them:

1. Spread vs. Rest: The transcript introduces the distinction between spread and rest. Spread is used to spread values or elements from a collection into separate individual elements, while rest is used to collect individual elements into a single collection.

2. Spread in function execution: Spread can be used when calling a function to spread an iterable into separate arguments. This allows passing individual values from an array as separate arguments to a function.

Code snippet (Spread array values as function arguments):
```javascript
function takesFour(one, two, three, four) {
  console.log(one, two, three, four);
}

const nums = [4, 5, 88, 123, 0.92];
takesFour(...nums); // Output: 4 5 88 123
```

3. Spread in console.log: Spread can be used with `console.log` to print each value of an array or string as separate arguments instead of printing the array or string itself.

Code snippet (Spread array and string values in console.log):
```javascript
const things = ['hello', 'world'];
console.log(...things); // Output: hello world

const str = 'HELLO';
console.log(...str); // Output: H E L L O
```

These code snippets demonstrate the usage of spread in function execution, where an iterable is spread into individual function arguments, and in `console.log` statements, where an array or string is spread to print each value as a separate argument.