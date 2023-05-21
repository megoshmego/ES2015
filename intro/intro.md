Important terms and ideas:

1. ES2015: Refers to ECMAScript 2015, which is a version of the ECMAScript standard. ES2015 introduced many new features and improvements to JavaScript, making it easier and more powerful for developers.

2. Browser Compatibility: Not all browsers fully support the newer features introduced in ES2015. Internet Explorer, in particular, has limited support for these features. It's important to consider browser compatibility when using ES2015 features.

3. ES6: Short for ECMAScript 6, ES6 is another name for ES2015. The term "ES6" is commonly used to refer to the version of ECMAScript that was released in 2015.

4. Blog Posts and Resources: There are various websites and blog posts that provide information and examples of ES2015 features. These resources help developers understand and learn about the new features introduced in ES2015.

Code snippet (Arrow Functions):

Here's a code snippet demonstrating the usage of arrow functions, one of the features introduced in ES2015:

```javascript
// ES2015: Arrow Functions
const add = (a, b) => a + b;
console.log(add(2, 3)); // Output: 5

const multiply = (a, b) => {
  const result = a * b;
  return result;
};
console.log(multiply(2, 3)); // Output: 6
```

Arrow functions provide a concise syntax for writing functions in JavaScript. They have implicit return and lexical scoping of `this`, making them useful for shorter function expressions.

Note that arrow functions may not be supported in older browsers or versions of JavaScript. To ensure compatibility, it's recommended to use a transpiler like Babel to convert ES2015 code into backward-compatible versions.

The transcript discusses the focus on newer features in JavaScript, specifically those introduced in ES2015. It mentions the importance of learning these features as they can make developers' lives easier. The transcript also acknowledges browser compatibility issues, particularly with Internet Explorer, and hints at addressing them. The mention of resources and websites to explore ES2015 features provides additional avenues for developers to deepen their understanding.