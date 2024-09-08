---
layout: base
title: Aranya Home
description: Home Page
hide: false
---
# JavaScript Cell - Math Jokes

Below is a JavaScript cell that outputs random math jokes to the console.

```javascript
// Array of math jokes
var mathJokeList = [
    { joke: "Why was the equal sign so humble? Because it knew it wasn't less than or greater than anyone else.", complexity: "O(1)" },
    { joke: "Why did the mathematician break up with his girlfriend? She had too many problems.", complexity: "O(1)" },
    { joke: "How do you stay warm in a cold room? Go to the corner, it’s always 90 degrees.", complexity: "O(1)" },
    { joke: "Why was the math book sad? It had too many problems.", complexity: "O(1)" },
    { joke: "Why was the fraction apprehensive about marrying the decimal? Because he would have to convert.", complexity: "O(1)" },
    { joke: "Why did the two fours skip lunch? They already eight.", complexity: "O(1)" },
    { joke: "What is a math teacher’s favorite place in NYC? Times Square.", complexity: "O(1)" },
    { joke: "Why was the student eating his math homework? Because his teacher said it was a piece of cake.", complexity: "O(1)" },
    { joke: "What do you call a number that can't keep still? A roamin' numeral.", complexity: "O(1)" },
    { joke: "Why was the obtuse triangle always so sad? Because it was never right.", complexity: "O(1)" }
];

// Get a random joke
var randomIndex = Math.floor(Math.random() * mathJokeList.length);
var selectedJoke = mathJokeList[randomIndex];
console.log("Math Joke #" + (randomIndex + 1) + ": " + selectedJoke.joke + " (Complexity: " + selectedJoke.complexity + ")");
