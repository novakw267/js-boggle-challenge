![General Assembly Logo](http://i.imgur.com/ke8USTq.png)

# Boggle challenge

## To start

Fork, clone, branch (challenge) and npm install

## Objective

Map row/column coordinates onto an array index (i.e. represent a square grid using a simple array).  Use this mapping to return (potential) words from letters in the grid.

## Activity

[Boggle](https://en.wikipedia.org/wiki/Boggle) is a word game played with letter-dice arrange in a 4X4 tray.

A _tray_ is just an array of length 16 with each element a single letter string.

A _list of coordinate pairs_ is an array with length <= 4 and each element is an array of length 2.  The sub-arrays contain two integers >= 0 and <= 3.

Write a function - in `lib/boggle.js` - that takes a **tray** and a **list of coordinate pairs** and returns a string representing the concatenation of the letters at each of the coordinates.

See `bin/boggle.js` for an example invocation.  Run it with `node bin/boggle.js`.  Run the tests with `grunt test`.

## Bonuses

### Big Boggle challenge

Big Boggle uses a 5X5 tray.

### Super Big Boggle challenge

Super Big Boggle uses a 6X6 tray.

### Validate inputs

- Ensure tray has the correct length
- Ensure that coordinates fall within the tray
- Disallow coordinate pairs that aren't in a line

Return the empty string if a validation fails

## [License](LICENSE)

Source code distributed under the MIT license. Text and other assets copyright
General Assembly, Inc., all rights reserved.
