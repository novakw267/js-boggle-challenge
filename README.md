![General Assembly Logo](http://i.imgur.com/ke8USTq.png)

# Boggle challenge

Test for words on a boggle board.

## Instructions

1.  Fork and clone this repository.
1.  Change into the new directory.
1.  Install dependencies.
1.  Create and checkout a new branch to work on.
1.  Fulfill the listed requirements.

Starter code is available in [`lib/challenge.js`](lib/challenge.js). A pull
request is not required, but it is necessary if you want a code review.

You may wish to refer to [FAQs](https://github.com/ga-wdi-boston/meta/wiki/)
related to [forking,
cloning](https://github.com/ga-wdi-boston/meta/wiki/ForkAndClone).

## Requirements

Map row/column coordinates onto an array index (i.e. represent a square grid
 using a simple array).  Use this mapping to return (potential) words from
 letters in the grid.

[Boggle](https://en.wikipedia.org/wiki/Boggle) is a word game played with
 letter-dice arrange in a 4X4 tray.

A _tray_ is just an array of length 16 with each element a single letter string.

A _list of coordinate pairs_ is an array with length <= 4 and each element is an
 array of length 2.  The sub-arrays contain two integers >= 0 and <= 3.

Write a function - in `lib/challenge.js` - that takes a **tray** and a **list of
 coordinate pairs** and returns a string representing the concatenation of the
 letters at each of the coordinates.

See `bin/challenge.js` for an example invocation.
Run it with `node bin/challenge.js`.

You should run `grunt nag` before diagnosing any bugs, since it finds some of
 the most common sources of errors.
After `grunt nag` passes, you should run `grunt test` to run the included tests.
Tests will tell you whether of not you've met these requirements.

## Bonuses

Only try these after completing the main challenge.

### Big Boggle challenge

Big Boggle uses a 5X5 tray.

Make the following change in `spec/challenge.spec.js` to enable tests for this
bonus.

```diff
- xdescribe('Big Boggle', () => {
+ describe('Big Boggle', () => {
```

### Super Big Boggle challenge

Super Big Boggle uses a 6X6 tray.

Make the following change in `spec/challenge.spec.js` to enable tests for this
bonus.

```diff
- xdescribe('Super Big Boggle', () => {
+ describe('Super Big Boggle', () => {
```

### Validate inputs

-   Ensure tray has the correct length
-   Ensure that coordinates fall within the tray
-   Disallow coordinate pairs that aren't in a line

Return the empty string if a validation fails

## [License](LICENSE)

Source code distributed under the MIT license. Text and other assets copyright
General Assembly, Inc., all rights reserved.
