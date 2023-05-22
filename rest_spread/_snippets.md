Certainly! Here are the code snippets that highlight the important concepts from the provided information:

1. Spread with object literals:
```javascript
const tea = {
  type: 'oolong',
  name: 'winter sprout',
  origin: 'Taiwan'
};

const tea2 = { ...tea };

console.log(tea2); // Output: { type: 'oolong', name: 'winter sprout', origin: 'Taiwan' }
```

2. Adding or updating properties:
```javascript
const tea = {
  type: 'oolong',
  name: 'winter sprout',
  origin: 'Taiwan'
};

const teaTin = { ...tea, price: 22.99 };

console.log(teaTin); // Output: { type: 'oolong', name: 'winter sprout', origin: 'Taiwan', price: 22.99 }
```

3. Order matters when spreading conflicting properties:
```javascript
const tea = {
  type: 'oolong',
  name: 'winter sprout',
  origin: 'Taiwan'
};

const newTea = { name: 'golden frost', ...tea };

console.log(newTea); // Output: { name: 'golden frost', type: 'oolong', origin: 'Taiwan' }
```

4. Combining objects with spread:
```javascript
const tea = {
  type: 'oolong',
  name: 'winter sprout',
  origin: 'Taiwan'
};

const teaData = {
  steepTime: '30s',
  brewTemp: 175
};

const fullTea = { ...tea, ...teaData };

console.log(fullTea);
// Output: { type: 'oolong', name: 'winter sprout', origin: 'Taiwan', steepTime: '30s', brewTemp: 175 }
```

5. Spreading arrays into objects:
```javascript
const colors = ['red', 'orange', 'blue'];
const dummyObject = { ...colors };

console.log(dummyObject);
// Output: { '0': 'red', '1': 'orange', '2': 'blue' }
```

6. Spreading strings into objects:
```javascript
const str = 'CAT';
const dummyObject = { ...str };

console.log(dummyObject);
// Output: { '0': 'C', '1': 'A', '2': 'T' }
```

These code snippets provide practical examples that showcase the usage of spread with object literals, including copying object properties, adding or updating properties, handling conflicting properties, combining objects, and the unusual behavior of spreading arrays and strings into objects.