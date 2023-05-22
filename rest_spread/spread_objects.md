Let's evaluate the important terms, ideas, and provide code snippets for each of them:

1. Spread with object literals: In addition to spreading array literals, we can also spread object literals. This involves copying properties from an existing object into a new object.

Code snippet (Spread object properties into a new object):
```javascript
const tea = {
  type: 'oolong',
  name: 'winter sprout',
  origin: 'Taiwan'
};

const tea2 = { ...tea };

console.log(tea2); // Output: { type: 'oolong', name: 'winter sprout', origin: 'Taiwan' }
```

2. Adding or updating properties: Spread can be used to create a new object based on an existing object while adding or updating specific properties.

Code snippet (Spread object properties and add a new property):
```javascript
const tea = {
  type: 'oolong',
  name: 'winter sprout',
  origin: 'Taiwan'
};

const teaTin = { ...tea, price: 22.99 };

console.log(teaTin); // Output: { type: 'oolong', name: 'winter sprout', origin: 'Taiwan', price: 22.99 }
```

3. Order matters when spreading conflicting properties: When spreading objects, the order of spreading properties matters. If there are conflicting property names, the last property assignment will overwrite previous ones.

Code snippet (Spread conflicting properties with different order):
```javascript
const tea = {
  type: 'oolong',
  name: 'winter sprout',
  origin: 'Taiwan'
};

const newTea = { name: 'golden frost', ...tea };

console.log(newTea); // Output: { name: 'golden frost', type: 'oolong', origin: 'Taiwan' }
```

4. Combining objects with spread: Spread can be used to combine multiple objects into a new object by spreading their properties into a new object.

Code snippet (Spread multiple objects into a new object):
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

5. Spreading arrays into objects: While it's uncommon, arrays can be spread into objects, resulting in properties with indices as keys.

Code snippet (Spreading an array into an object):
```javascript
const colors = ['red', 'orange', 'blue'];
const dummyObject = { ...colors };

console.log(dummyObject);
// Output: { '0': 'red', '1': 'orange', '2': 'blue' }
```

6. Spreading strings into objects: Strings, despite being primitives, can be spread into objects, resulting in properties with indices as keys.

Code snippet (Spreading a string into an object):
```javascript
const str = 'CAT';
const dummyObject = { ...str };

console.log(dummyObject);
// Output: { '0': 'C', '1': 'A', '2': 'T' }
```

These code snippets demonstrate the usage of spread with object literals, including copying object properties, adding or updating properties, handling conflicting properties, combining objects, and the unusual behavior of spreading arrays and strings into objects.