The important terms and ideas discussed in the transcript are:

1. Object property shorthand: It refers to a shorthand syntax for creating object literals where the property names and their values can be defined using variables of the same name.

Here's a simple demonstration of object property shorthand:

```javascript
// Without shorthand
const firstName = 'Jim';
const lastName = 'Lennon';
const age = 29;

const person = {
  firstName: firstName,
  lastName: lastName,
  age: age
};

console.log(person); // Output: { firstName: 'Jim', lastName: 'Lennon', age: 29 }

// With shorthand
const firstName = 'Jim';
const lastName = 'Lennon';
const age = 29;

const person = {
  firstName,
  lastName,
  age
};

console.log(person); // Output: { firstName: 'Jim', lastName: 'Lennon', age: 29 }
```

In the example, the shorthand syntax is used to create an object literal `person` with properties assigned using the variables `firstName`, `lastName`, and `age`. The shorthand reduces the duplication of property names and variable names, making the code more concise.

The object property shorthand is widely supported in modern browsers, except for Internet Explorer. Transpilation tools like Babel can be used to convert the shorthand syntax to a compatible form for older browsers.

This enhancement provides a convenient way to create objects with property names derived from variable names.

Overall, the shorthand property names allow for cleaner and more concise code when creating object literals.