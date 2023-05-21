Condensed information:

1. Hoisting: JavaScript behavior where variable declarations are moved to the top of their scope during compilation, allowing variables to be accessed before they are declared.
2. var: Keyword for declaring variables with function scope or global scope. Variables are hoisted and can lead to unexpected behavior.
3. let: Keyword for declaring block-scoped variables. Not hoisted and initialized at the code execution point.
4. const: Keyword for declaring block-scoped variables that cannot be reassigned. Not hoisted and must be assigned an initial value at declaration.

Code snippets:

1. Variable Hoisting with var:
```javascript
var chickens;
console.log(chickens); // Output: undefined
chickens = ['Hen', 'Rooster'];
console.log(chickens); // Output: ['Hen', 'Rooster']
```

2. No Variable Hoisting with let:
```javascript
let chickens;
console.log(chickens); // Error: Cannot access 'chickens' before initialization
chickens = ['Hen', 'Rooster'];
console.log(chickens);
```

3. Missing Initializer in const Declaration:
```javascript
const fish; // Error: Missing initializer in const declaration
let bird;
bird = 'Sparrow';
const cat = 'Tom';
```

4. Using const:
```javascript
const count = 0;
console.log(count); // Output: 0

count = 1; // Error: Assignment to constant variable
```

5. Using let:
```javascript
let count = 0;
console.log(count); // Output: 0

count += 1;
console.log(count); // Output: 1
```

6. Avoiding var:
```javascript
let age = 25;

if (age >= 18) {
  let status = 'adult';
}

console.log(status); // Output: ReferenceError: status is not defined
```

7. Variable Scope with var:
```javascript
var song = 'Goodbye Yellow Brick Road';

function sing() {
  console.log(song);
}

sing(); // Output: 'Goodbye Yellow Brick Road'
console.log(song); // Output: 'Goodbye Yellow Brick Road'
```

8. Variable Re-declaration with var:
```javascript
var musician = 'Elton John';
console.log(musician); // Output: 'Elton John'

var musician = 'Alanis Morissette';
console.log(musician); // Output: 'Alanis Morissette'
```

9. Variable Hoisting with var:
```javascript
var song;
console.log(song); // Output: undefined
song = 'Goodbye Yellow Brick Road';
console.log(song); // Output: 'Goodbye Yellow Brick Road'
```

10. Variable Reassignment with let:
```javascript
let x = 10;
console.log(x); // Output: 10

x = 20;
console.log(x); // Output: 20
```

11. Variable Redeclaration with let:
```javascript
let x = 10;
console.log(x); // Output: 10

let x = 20; // Error: Identifier 'x' has already been declared
```

12. Block Scope with let:
```javascript
let color = 'teal';

if (true) {
  let color = 'blue';
  console.log(color); // Output: 'blue'
}

console.log(color); // Output: 'teal'
```

13. Variable Reassignment with const:
```javascript
const x = 10;
console.log(x); // Output: 10

x = 20; // Error: Assignment to constant variable
```
Certainly! Here's the continuation:

14. Mutating Contents with const:
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

The information and code snippets provided cover the important concepts related to hoisting, variable declaration with `var`, `let`, and `const`, as well as the behavior of each keyword. The code snippets demonstrate hoisting, reassignment, redeclaration, block scoping, and the mutability of non-primitive types with `const`.