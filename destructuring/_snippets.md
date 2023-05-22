Certainly! Here are code snippets that can be helpful for learning the discussed concepts:

**1. Destructuring Arrays:**
```javascript
const students = [
  { name: 'Drake', GPA: 4.6 },
  { name: 'Henrietta', GPA: 4.4 },
  { name: 'Tung', GPA: 3.9 },
  { name: 'Harry', GPA: 4.2 },
  { name: 'Sarah', GPA: 4.1 }
];

const [topStudent, secondBest, , fourth] = students;

console.log(topStudent); // Output: { name: 'Drake', GPA: 4.6 }
console.log(secondBest); // Output: { name: 'Henrietta', GPA: 4.4 }
console.log(fourth); // Output: { name: 'Harry', GPA: 4.2 }
```

**2. Skipping Array Elements:**
```javascript
const students = ['Drake', 'Henrietta', 'Tung', 'Harry', 'Sarah'];

const [, , , fourth] = students;

console.log(fourth); // Output: 'Harry'
```

**3. Rest Operator with Arrays:**
```javascript
const students = ['Drake', 'Henrietta', 'Tung', 'Harry', 'Sarah'];

const [first, ...losers] = students;

console.log(first); // Output: 'Drake'
console.log(losers); // Output: ['Henrietta', 'Tung', 'Harry', 'Sarah']
```

**4. Swapping Variables:**
```javascript
let delicious = 'mayonnaise';
let disgusting = 'whipped cream';

[delicious, disgusting] = [disgusting, delicious];

console.log(delicious); // Output: 'whipped cream'
console.log(disgusting); // Output: 'mayonnaise'
```

**5. Destructuring in Function Parameters (Object):**
```javascript
function getTotal({ quantity = 1, price }) {
  return quantity * price;
}

const order = {
  price: 12.99,
  quantity: 3
};

console.log(getTotal(order)); // Output: 38.97
```

**6. Destructuring in Function Parameters (Array):**
```javascript
function awardMedals([gold, silver, bronze]) {
  return { gold, silver, bronze };
}

const longJumpResults = ['Tammy', 'Jessica', 'Violet'];

console.log(awardMedals(longJumpResults));
// Output: { gold: 'Tammy', silver: 'Jessica', bronze: 'Violet' }
```

**7. Nested Destructuring (Object):**
```javascript
const instructor = {
  name: 'John',
  funFacts: {
    favoriteFood: 'Pizza',
    favoriteDrink: 'Coffee'
  }
};

const { funFacts: { favoriteFood, favoriteDrink } } = instructor;

console.log(favoriteFood); // Output: Pizza
console.log(favoriteDrink); // Output: Coffee
```

**8. Nested Destructuring (Array):**
```javascript
const movie = {
  ratings: [
    { source: 'IMDB', value: 8.3 },
    { source: 'Rotten Tomatoes', value: '93%' },
    { source: 'Metacritic', value: '88 out of 100' }
  ],
  versions: [
    { type: 'Original', runtime: 161 },
    { type: "Director's Cut", runtime: 180 }
  ]
};

const { ratings: [{ value: imdbRating }, , { value: rottenTomatoes