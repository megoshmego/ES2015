Important terms and ideas:

1. const: A keyword introduced in ES6 for declaring block-scoped variables. Variables declared with `const` have block scope and cannot be reassigned once they are assigned an initial value. However, for non-primitive types like arrays and objects, the contents can be mutated while keeping the same reference.

2. Block scope: Refers to the scope of variables within a block of code, such as a loop or conditional statement. `const` variables, like `let` variables, have block scope, meaning they are accessible only within the block they are defined in.

3. Reassignment: Refers to changing the value of a variable after it has been declared. `const` variables cannot be reassigned once they are assigned an initial value. Reassigning a `const` variable will result in a type error.

4. Redeclaration: Refers to declaring another variable with the same name within the same scope. Like `let` variables, `const` variables cannot be redeclared within the same scope.

5. Mutability: Refers to the ability to change the contents or properties of a variable. While `const` variables cannot be reassigned, they can still have their contents or properties mutated for non-primitive types like arrays and objects.

6. Hoisting: An advanced JavaScript concept where variable and function declarations are moved to the top of their containing scope during the compilation phase, allowing them to be accessed before they are declared. However, hoisting does not work the same way for `let` and `const` variables as it does for `var` variables.

Code snippet (Variable Reassignment with const):

```javascript
const x = 10;
console.log(x); // Output: 10

x = 20; // Error: Assignment to constant variable
```

In this code snippet, the variable `x` is declared with `const` and assigned a value. An attempt to reassign `x` to a different value results in a type error. Reassignment is not allowed for `const` variables.

Code snippet (Mutating Contents with const):

```javascript
const myCats = [];
myCats.push('Monty');
console.log(myCats); // Output: ['Monty']

myCats[0] = 'Rockets';
console.log(myCats); // Output: ['Rockets']
```

In this code snippet, the variable `myCats` is declared with `const` and assigned an empty array. Although the variable cannot be reassigned, the contents of the array can be mutated using methods like `push` or by directly accessing and modifying array elements.

Code snippet (Block Scope with const):

```javascript
if (true) {
  const PI = 3.14;
  console.log(PI); // Output: 3.14
}

console.log(PI); // Error: PI is not defined
```

In this code snippet, the variable `PI` is declared with `const` within the if statement block. The variable is accessible only within that block due to block scoping. An attempt to access `PI` outside the block results in an error.

The transcript explains the concept of `const` variables in JavaScript. It highlights that `const` variables are block-scoped and cannot be reassigned or redeclared within the same scope. It discusses the ability to mutate the contents of non-primitive types like arrays and objects while keeping the same reference. The code snippets demonstrate the behaviors of reassignment, mutation, and block scope with `const` variables.