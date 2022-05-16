[![General Assembly Logo](https://camo.githubusercontent.com/1a91b05b8f4d44b5bbfb83abac2b0996d8e26c92/687474703a2f2f692e696d6775722e636f6d2f6b6538555354712e706e67)](https://generalassemb.ly/education/web-development-immersive)

# Array Iterator Methods Lab

## Intro

You've been introduced to the very useful array iterator methods `forEach` and `map`.

The following exercises provide practice using some of them. There are bonus exercises that require you to read about additional methods and implement them.

## Set Up

1. Create a directory called `array-methods-lab` in your `sei/labs` folder and set up an HTML and JS environment.

2. Copy the code below into the JavaScript file and complete each exercise.

## Instructions

- `console.log` each exercise's answer

- Verify your `console.log` output matches that shown at the bottom.

## Suggestion

Be sure to stub up the skeleton of the code. Then you can "flesh" it out.

For example, if asked to return an array of strings that say "I want a `toy name`" for every element in the toys array:

```js
// Stub up the skeleton of the code...
const wishList = toys.map(function (toy) {});
```

Then, flesh out the callback function...

```js
const wishList = toys.map(function (toy) {
	return `I want a ${toy}`;
});
```

## Exercises

```js
const inventors = [
	{ first: 'Albert', last: 'Einstein', year: 1879, passed: 1955 },
	{ first: 'Isaac', last: 'Newton', year: 1643, passed: 1727 },
	{ first: 'Galileo', last: 'Galilei', year: 1564, passed: 1642 },
	{ first: 'Marie', last: 'Curie', year: 1867, passed: 1934 },
	{ first: 'Johannes', last: 'Kepler', year: 1571, passed: 1630 },
	{ first: 'Nicolaus', last: 'Copernicus', year: 1473, passed: 1543 },
	{ first: 'Max', last: 'Planck', year: 1858, passed: 1947 },
	{ first: 'Katherine', last: 'Blodgett', year: 1898, passed: 1979 },
	{ first: 'Ada', last: 'Lovelace', year: 1815, passed: 1852 },
	{ first: 'Sarah E.', last: 'Goode', year: 1855, passed: 1905 },
	{ first: 'Lise', last: 'Meitner', year: 1878, passed: 1968 },
	{ first: 'Hanna', last: 'Hammarström', year: 1829, passed: 1909 },
];

// Array.prototype.forEach()
// 1. Log each inventor and the year they were born in a string: e.g., "Albert Einstein was born in 1879."

// Array.prototype.map()
// 2. Map the array of inventors into a new array of numbers containing how long each inventor lived.

// Array.prototype.map()
// 3.  Map the array of the inventors into a new array containing objects with just the first and last names as properties
// Hint:  Return a new object literal from the callback (don't mutate the object being passed in to map)

// Array.prototype.filter()
// 4. Filter the array of inventors into a new array containing only the inventors born in the 1500's
// Hint: Be sure to check out the MDN documentation on .filter()

const people = [
	'Becker, Carl',
	'Beckett, Samuel',
	'Beddoes, Mick',
	'Beecher, Henry',
	'Beethoven, Ludwig',
	'Begin, Menachem',
	'Belloc, Hilaire',
	'Bellow, Saul',
	'Benchley, Robert',
	'Benenson, Peter',
	'Ben-Gurion, David',
	'Benjamin, Walter',
	'Benn, Tony',
	'Bennington, Chester',
	'Benson, Leana',
	'Bent, Silas',
	'Bentsen, Lloyd',
	'Berger, Ric',
	'Bergman, Ingmar',
	'Berio, Luciano',
	'Berle, Milton',
	'Berlin, Irving',
	'Berne, Eric',
	'Bernhard, Sandra',
	'Berra, Yogi',
	'Berry, Halle',
	'Berry, Wendell',
	'Bethea, Erin',
	'Bevan, Aneurin',
	'Bevel, Ken',
	'Biden, Joseph',
	'Bierce, Ambrose',
	'Biko, Steve',
	'Billings, Josh',
	'Biondo, Frank',
	'Birrell, Augustine',
	'Black, Elk',
	'Blair, Robert',
	'Blair, Tony',
	'Blake, William',
];

// Array.prototype.map()
// 5. Map the people array such that the new array consists of strings with the names formatted as "First Last", e.g., "Becker, Carl" should be mapped to "Carl Becker".
// Hint: As a start, consider using the String.prototype.split method to "split" the string using ', ' as the separator

const comments = [
	{ text: 'Love this!', id: 523423 },
	{ text: 'Super good', id: 823423 },
	{ text: 'You are the best', id: 2039842 },
	{ text: 'Ramen is my fav food ever', id: 123523 },
	{ text: 'Nice Nice Nice!', id: 542328 },
];

// Array.prototype.map()
// 6. Map the comments array and return a new array that logs a string that says `User <id> says: "text"`. For example, `User 523423 says "Love this!"`
```

## Verify `console.log` Output

```js
// 1.
// Albert Einstein was born in 1879.
// Isaac Newton was born in 1643.
// Galileo Galilei was born in 1564.
// Marie Curie was born in 1867.
// Johannes Kepler was born in 1571.
// Nicolaus Copernicus was born in 1473.
// Max Planck was born in 1858.
// Katherine Blodgett was born in 1898.
// Ada Lovelace was born in 1815.
// Sarah E. Goode was born in 1855.
// Lise Meitner was born in 1878.
// Hanna Hammarström was born in 1829.

// 2.
// [ 76, 84, 78, 67, 59, 70, 89, 81, 37, 50, 90, 80 ]

// 3.
// [
//   { first: 'Albert', last: 'Einstein' },
//   { first: 'Isaac', last: 'Newton' },
//   { first: 'Galileo', last: 'Galilei' },
//   { first: 'Marie', last: 'Curie' },
//   { first: 'Johannes', last: 'Kepler' },
//   { first: 'Nicolaus', last: 'Copernicus' },
//   { first: 'Max', last: 'Planck' },
//   { first: 'Katherine', last: 'Blodgett' },
//   { first: 'Ada', last: 'Lovelace' },
//   { first: 'Sarah E.', last: 'Goode' },
//   { first: 'Lise', last: 'Meitner' },
//   { first: 'Hanna', last: 'Hammarström' }
// ]

// 4.
// [
//   { first: 'Galileo', last: 'Galilei', year: 1564, passed: 1642 },
//   { first: 'Johannes', last: 'Kepler', year: 1571, passed: 1630 }
// ]

// 5.
// [
//   'Carl Becker',      'Samuel Beckett',
//   'Mick Beddoes',     'Henry Beecher',
//   'Ludwig Beethoven', 'Menachem Begin',
//   'Hilaire Belloc',   'Saul Bellow',
//   'Robert Benchley',  'Peter Benenson',
//   'David Ben-Gurion', 'Walter Benjamin',
//   'Tony Benn',        'Chester Bennington',
//   'Leana Benson',     'Silas Bent',
//   'Lloyd Bentsen',    'Ric Berger',
//   'Ingmar Bergman',   'Luciano Berio',
//   'Milton Berle',     'Irving Berlin',
//   'Eric Berne',       'Sandra Bernhard',
//   'Yogi Berra',       'Halle Berry',
//   'Wendell Berry',    'Erin Bethea',
//   'Aneurin Bevan',    'Ken Bevel',
//   'Joseph Biden',     'Ambrose Bierce',
//   'Steve Biko',       'Josh Billings',
//   'Frank Biondo',     'Augustine Birrell',
//   'Elk Black',        'Robert Blair',
//   'Tony Blair',       'William Blake'
// ]

// 6.
// [
//   'User 523423 says: Love this!',
//   'User 823423 says: Super good',
//   'User 2039842 says: You are the best',
//   'User 123523 says: Ramen is my fav food ever',
//   'User 542328 says: Nice Nice Nice!'
// ]
```

## Reference

[Array Reference on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)

## Attribution

Adapted from a resource created by Jim Clark.
