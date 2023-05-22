The important terms and ideas discussed in the transcript are:

1. Data Structures: Data structures are ways of storing and organizing multiple pieces of data.
2. Arrays and Objects: Prior to the introduction of maps and sets in JavaScript, arrays and objects were the primary data structures for storing multiple values.
3. Maps: Maps are data structures that store key-value pairs. They are similar to JavaScript objects but have some important distinctions.
4. Key-Value Pairs: Maps store data in key-value pairs, where each key is associated with a corresponding value.
5. Keys in Maps: Unlike objects, keys in maps can be any data type and are not automatically converted to strings.
6. `new Map()`: The `new Map()` syntax is used to create an empty map.
7. `set()` method: The `set()` method is used to add key-value pairs to a map.
8. Retrieving Values: The `get()` method is used to retrieve the value associated with a specific key in a map.
9. Usage of Different Data Types as Keys: Maps allow any data type to be used as a key, including numbers, strings, objects, arrays, functions, and booleans.

**Simple Demonstrations:**

1. Creating a Map and Setting Key-Value Pairs:
```javascript
const myMap = new Map();
myMap.set(7, 'Seven');
myMap.set('7', 'Seven String');
myMap.set([], 'Empty Array');
myMap.set(true, 'True Value');
myMap.set({ key: 'value' }, 'Object');
myMap.set(function () { }, 'Function');

console.log(myMap);
```

2. Retrieving Values from a Map:
```javascript
console.log(myMap.get(7)); // Output: Seven
console.log(myMap.get('7')); // Output: Seven String
console.log(myMap.get([])); // Output: Empty Array
console.log(myMap.get(true)); // Output: True Value
console.log(myMap.get({ key: 'value' })); // Output: undefined
console.log(myMap.get(function () { })); // Output: undefined
```

3. Using Object References as Keys:
```javascript
const emptyArray = [];
myMap.set(emptyArray, 'Empty Array Reference');
console.log(myMap.get(emptyArray)); // Output: Empty Array Reference
```

These demonstrations show how different data types can be used as keys in a map and how to retrieve corresponding values.