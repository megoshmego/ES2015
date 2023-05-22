The important terms and ideas discussed in the transcript are:

1. Object methods: Methods are functions that are stored as properties in an object. They allow us to add functions as properties in an object literal.

Here's a simple demonstration of object methods:

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

In the example, `mathStuff` is an object with two properties, `add` and `square`, which are defined as functions. These functions can be called as methods on the `mathStuff` object, and they perform the respective mathematical operations.

2. Shorthand method syntax: Instead of using the `function` keyword to define methods, we can use a shorthand syntax where we directly write the function name, parameters, and body inside the object literal.

Here's a demonstration of the shorthand method syntax:

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

In the example, the methods `add` and `square` are defined using the shorthand syntax. This syntax is more concise and resembles regular function declarations.

It's important to note that arrow functions cannot be used as shorthand methods because arrow functions do not have their own `this` binding. Regular functions are recommended for object methods.

The shorthand method syntax is supported by modern browsers, but it is not supported in Internet Explorer. Transpilation tools like Babel can be used to convert the shorthand syntax to a compatible form for older browsers.

Overall, the shorthand method syntax provides a cleaner and more concise way to define methods in object literals.