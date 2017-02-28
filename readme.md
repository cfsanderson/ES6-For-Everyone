# My notes below...

## Section 01
### Video 01
- `var` variables are globally scoped unless inside a function in which they are in "bracket jail" = function scoped but does NOT apply to other brackets (e.g. an `if` statement).
- `let` and `const` variables are both BLOCK scoped meaning they are scoped to the block (whatever brackets) they are in.

### Video 02
- Cannot redeclare a `let` variable in the same scope the way you can with `var`
- `const` cannot be changed (as in "constant") but it's properties CAN be updated.

### Video 04
Temporal dead zone = you cannot access a variable before it has been defined

### Video 0
when to use `var`/`let`/`const`
  - use `const` by default
  - only use `let` if rebinding is needed
  - (`var` shouldn't be used)

### Video 06
Arrow functions - 3 main reasons to use...
  - more concise
  - implicit returns (1 liners easy)
  - doesn't rebind `this` when you use inside another function (e.g. in click handlers)




![ES6 for Everyone](https://es6.io/images/es6-facebook-share.png?cool=yah)
