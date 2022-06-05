## Project 2

In this project we used the CLI to create and use a git repository. We refactored our JS code from the Project 1 to practice using git and refactoring.

Technologies used for this project:
- VSCode
- CLI
- git

The purpose of this project was to gain experince using git through out CLI and VSCode, writing/ executing server side Node.js Javascript code, and practice refactoring.

From doing this project I learned how to refactor my code to be simpler and more efficent when looking at it. I also learned how to create a .gitignore file.

```
/*
    CIT 281 Project 1
    Name: Olivia Edwards
*/

// Returns a random number between min (inclusive) and max (exclusive)
const getRandomInteger = function(min, max) {
    return Math.floor(Math.random() * (max - min) + min);
}

// Returns a single random lowercase letter from an array of the alphabet
const getRandomLetter = function() {
    let randomLetter = getRandomInteger(0, 27);
    const alphabet = "abcdefghijklmnopqrstuvwxyz".split("");
    return alphabet[randomLetter];
}
//const alphabet = "abcdefghijklmnopqrstuvwxyz".split("");

//returns random string of lowercase letters 
const getRandomString = function(minLength, maxLength) {
    maxLength += 1;
    let stringLength = getRandomInteger(minLength, maxLength);
    let result = "";
    for (let i = 0; i < stringLength; i++) {
        result += getRandomLetter();
    }
    return result;
}

//takes a string of randomly arranged letters and returns them in ascending order
const getSortedString = function(string) {
  return (string.split("")).sort().join("");
}
//let result = "";

//let lengthOfOutputString = getRandomInteger(5, 26);

//for (let i = 0; i < lengthOfOutputString; i++) {
  //result += getRandomLetter();
//}

console.log(getSortedString(getRandomString(10, 20)));
```

```
/*
    CIT 281 Project 1
    Name: Olivia Edwards
*/

// Returns a random number between min (inclusive) and max (exclusive)
function getRandomInteger(min, max) {
    return Math.floor(Math.random() * (max - min) + min);
}

// Returns a single random lowercase letter from an array of the alphabet
function getRandomLetter() {
    let randomLetter = getRandomInteger(0, 27);
    const alphabet = "abcdefghijklmnopqrstuvwxyz".split("");
    return alphabet[randomLetter];
}
//const alphabet = "abcdefghijklmnopqrstuvwxyz".split("");

//returns random string of lowercase letters 
function getRandomString(minLength, maxLength) {
    maxLength += 1;
    let stringLength = getRandomInteger(minLength, maxLength);
    let result = "";
    for (let i = 0; i < stringLength; i++) {
        result += getRandomLetter();
    }
    return result;
}

//takes a string of randomly arranged letters and returns them in ascending order
function getSortedString(string) {
  return (string.split("")).sort().join("");
}
//let result = "";

//let lengthOfOutputString = getRandomInteger(5, 26);

//for (let i = 0; i < lengthOfOutputString; i++) {
  //result += getRandomLetter();
//}

console.log(getSortedString(getRandomString(10, 20)));
```
