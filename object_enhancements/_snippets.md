Here are code snippets that can be helpful for learning the material:

Snippet 1: Object methods
```javascript
const mathStuff = {
  add: function(a, b) {
    return a + b;
  },
  square: function(a) {
    return a ** 2;
  }
};

console.log(mathStuff.add(3, 7)); // Output: 10
console.log(mathStuff.square(9)); // Output: 81
```

Snippet 2: Shorthand method syntax
```javascript
const mathStuff = {
  add(a, b) {
    return a + b;
  },
  square(a) {
    return a ** 2;
  }
};

console.log(mathStuff.add(3, 7)); // Output: 10
console.log(mathStuff.square(9)); // Output: 81
```

Snippet 3: Object property shorthand
```javascript
const firstName = 'Jim';
const lastName = 'Lennon';
const age = 29;

// Without shorthand
const person = {
  firstName: firstName,
  lastName: lastName,
  age: age
};

console.log(person); // Output: { firstName: 'Jim', lastName: 'Lennon', age: 29 }

// With shorthand
const person = {
  firstName,
  lastName,
  age
};

console.log(person); // Output: { firstName: 'Jim', lastName: 'Lennon', age: 29 }
```

Snippet 4: Computed property names
```javascript
const name = 'bright ube';
const hex = '#D6A2E8';

const color = {
  [name]: hex,
  [hex]: name
};

console.log(color['bright ube']); // Output: #D6A2E8
console.log(color['#D6A2E8']); // Output: bright ube
```

These snippets demonstrate the concepts discussed in the transcript, providing practical examples of object methods, shorthand method syntax, object property shorthand, and computed property names.