Important terms and ideas:

1. let: A keyword introduced in ES6 for declaring block-scoped variables that can be reassigned.

2. const: A keyword introduced in ES6 for declaring block-scoped variables that cannot be reassigned.

3. var: A keyword for declaring variables with function scope or global scope. It is considered outdated and should be avoided in modern JavaScript.

Code snippet (Using const):

```javascript
// Example using const
const count = 0;
console.log(count); // Output: 0

// Cannot reassign const variables
count = 1; // Error: Assignment to constant variable
```

In this code snippet, the variable `count` is declared using `const` and assigned an initial value of 0. The `count` variable cannot be reassigned, as demonstrated by the error when attempting to assign a new value to it.

Code snippet (Using let):

```javascript
// Example using let
let count = 0;
console.log(count); // Output: 0

// Reassigning let variables
count += 1;
console.log(count); // Output: 1
```

In this code snippet, the variable `count` is declared using `let` and assigned an initial value of 0. Unlike `const`, `let` variables can be reassigned, as shown by incrementing the `count` variable.

Code snippet (Avoiding var):

```javascript
// Example avoiding var
let age = 25; // Preferred over var

if (age >= 18) {
  var status = 'adult'; // Avoid using var
}

console.log(status); // Output: adult
```

In this code snippet, the variable `age` is declared using `let`, which is the preferred way of declaring variables in modern JavaScript. The `status` variable is declared using `var`, but it's generally recommended to use `let` or `const` instead of `var` due to its function scope or global scope behavior. However, it's important to note that `status` is accessible outside the `if` block due to the hoisting behavior of `var`.