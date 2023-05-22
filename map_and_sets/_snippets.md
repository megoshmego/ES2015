

**Code Snippets:**

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

4. Iterating over a Map with `for...each`:
```javascript
const bandMap = new Map();
bandMap.set(3, '3 Doors Down');
bandMap.set(9, 'Nine Inch Nails');

bandMap.forEach((value, key) => {
  console.log(`${key} = ${value}`);
});
```

5. Iterating over a Map with `for...of`:
```javascript
const bandMap = new Map();
bandMap.set(3, '3 Doors Down');
bandMap.set(9, 'Nine Inch Nails');

for (const [key, value] of bandMap) {
  console.log(`${key} = ${value}`);
}
```

6. Iterating over Keys:
```javascript
const bandMap = new Map();
bandMap.set(3, '3 Doors Down');
bandMap.set(9, 'Nine Inch Nails');

for (const key of bandMap.keys()) {
  console.log(key);
}
```

7. Iter

ating over Values:
```javascript
const bandMap = new Map();
bandMap.set(3, '3 Doors Down');
bandMap.set(9, 'Nine Inch Nails');

for (const value of bandMap.values()) {
  console.log(value);
}
```

8. Using Sets:
```javascript
const set = new Set();
set.add('apple');
set.add('banana');
set.add('apple'); // Ignored, already exists

console.log(set); // Output: Set(2) { 'apple', 'banana' }
```

9. Checking Value Existence in a Set:
```javascript
const set = new Set(['apple', 'banana', 'orange']);
console.log(set.has('apple')); // Output: true
console.log(set.has('grape')); // Output: false
```

10. Deleting Values from a Set:
```javascript
const set = new Set(['apple', 'banana', 'orange']);
console.log(set.delete('banana')); // Output: true
console.log(set.delete('grape')); // Output: false
console.log(set); // Output: Set(2) { 'apple', 'orange' }
```

11. Clearing a Set:
```javascript
const set = new Set(['apple', 'banana', 'orange']);
set.clear();

console.log(set); // Output: Set(0) {}
```

These code snippets demonstrate the concepts discussed in the transcript, including maps, sets, adding values, retrieving values, deleting values, clearing sets, iterating over maps and sets, and checking value existence.