The important terms and ideas discussed in the transcript are:

1. Iterating over a Map: There are two methods to iterate over a map - `for...of` and `for...each`.
2. Map Order: Maps are ordered data structures, and the order of elements is based on the insertion order.
3. Map Size: Maps have a `size` property that indicates the number of key-value pairs in the map.
4. Object vs. Map: Maps provide a reliable order and have a `size` property, unlike objects. Objects are trickier to iterate over compared to maps.
5. `for...each` with Map: The `for...each` method can be used to iterate over a map, with the first parameter in the callback representing the value and the second parameter representing the key.
6. `for...of` with Map: The `for...of` method can be used to iterate over a map, and each iteration returns an array where the first element is the key and the second element is the value.

**Simple Demonstrations:**

1. `for...each` with Map:
```javascript
const bandMap = new Map();
bandMap.set(3, '3 Doors Down');
bandMap.set(9, 'Nine Inch Nails');

bandMap.forEach((value, key) => {
  console.log(`${key} = ${value}`);
});
```

2. `for...of` with Map:
```javascript
const bandMap = new Map();
bandMap.set(3, '3 Doors Down');
bandMap.set(9, 'Nine Inch Nails');

for (const [key, value] of bandMap) {
  console.log(`${key} = ${value}`);
}
```

3. Iterating over Keys:
```javascript
const bandMap = new Map();
bandMap.set(3, '3 Doors Down');
bandMap.set(9, 'Nine Inch Nails');

for (const key of bandMap.keys()) {
  console.log(key);
}
```

4. Iterating over Values:
```javascript
const bandMap = new Map();
bandMap.set(3, '3 Doors Down');
bandMap.set(9, 'Nine Inch Nails');

for (const value of bandMap.values()) {
  console.log(value);
}
```