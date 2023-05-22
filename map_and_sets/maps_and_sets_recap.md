The important terms and ideas discussed in the transcript are:

1. Set: A data structure in JavaScript that stores unique values.
2. Unique Values: Sets only store unique values, meaning duplicates are not allowed.
3. Literal Syntax: Sets are created using the `new Set()` syntax.
4. Efficiency: Sets are more efficient than arrays for certain operations like looking up values and adding new values.
5. Adding Values: Values can be added to a set using the `add()` method.
6. Checking Value Existence: The `has()` method is used to check if a value exists in a set.
7. Deleting Values: The `delete()` method removes a specific value from a set.
8. Clearing a Set: The `clear()` method removes all values from a set.
9. Mimicking Sets with Arrays: While arrays can replicate some set functionality, using sets is more efficient for checking value existence.
10. Removing Duplicates: Sets can easily remove duplicates from an array by converting it to a set and then back to an array.
11. Iterating with Sets: Sets have three commonly used methods: `add()`, `delete()`, and `has()`.
12. Iterating with Sets: Sets can store various types of values, as long as they are unique.

**Simple Demonstrations:**

1. Creating a Set:
```javascript
const set = new Set();
console.log(set); // Output: Set(0) {}
```

2. Adding Values to a Set:
```javascript
const set = new Set();
set.add('apple');
set.add('banana');
set.add('apple'); // Ignored, already exists

console.log(set); // Output: Set(2) { 'apple', 'banana' }
```

3. Checking Value Existence:
```javascript
const set = new Set(['apple', 'banana', 'orange']);
console.log(set.has('apple')); // Output: true
console.log(set.has('grape')); // Output: false
```

4. Deleting a Value:
```javascript
const set = new Set(['apple', 'banana', 'orange']);
console.log(set.delete('banana')); // Output: true
console.log(set.delete('grape')); // Output: false
console.log(set); // Output: Set(2) { 'apple', 'orange' }
```

5. Clearing a Set:
```javascript
const set = new Set(['apple', 'banana', 'orange']);
set.clear();

console.log(set); // Output: Set(0) {}
```

6. Removing Duplicates from an Array:
```javascript
const array = [1, 2, 3, 2, 1];
const uniqueArray = [...new Set(array)];

console.log(uniqueArray); // Output: [1, 2, 3]
```

These code snippets demonstrate the concepts discussed in the transcript, including creating sets, adding values, checking value existence, deleting values, clearing sets, mimicking sets with arrays, removing duplicates, and iterating with sets.