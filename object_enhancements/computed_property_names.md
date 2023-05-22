The important terms and ideas discussed in the transcript are:

1. Computed property names: Computed property names allow us to add dynamic keys to an object, where the key name is based on a variable or an expression, rather than being a hardcoded string.

Here's a simple demonstration of computed property names:

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

In the example, the keys of the `color` object are computed based on the values of the `name` and `hex` variables. The square brackets `[]` are used to define the dynamic key names within the object literal.

Computed property names provide a more concise and expressive way to create objects with dynamic keys. They can be used for one-liners or with code expressions inside the brackets.

It's important to note that computed property names are not supported in Internet Explorer, but they are supported in other modern browsers. Transpilation tools like Babel can be used to convert the code with computed property names to a compatible form for older browsers.

Overall, computed property names allow for more flexibility and dynamic object creation by using variables and expressions to determine the key names.