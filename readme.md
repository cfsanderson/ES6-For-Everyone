# My notes below...

## Section 01
### Video 01
- `var` variables are globally scoped unless inside a function in which they are in "bracket jail" = function scoped but does NOT apply to other brackets (e.g. an `if` statement).
- `let` and `const` variables are both BLOCK scoped meaning they are scoped to the block (whatever brackets) they are in.

### Video 02
- Cannot redeclare a `let` variable in the same scope the way you can with `var`
- A `const` variable cannot be changed (as in "constant") but it's properties CAN be updated.

### Video 03
- an IIFE (Immediately-Invoked Function Expression) which is a function that runs before anything else and prevents variables leaking (e.g. `var name = "Caleb"`) is not necessary any longer since `let` and `const` are block scoped. Simply put them in brackets.
- in a `for` loop if you use `var i = 0` var is overwritten every time it loops so after the last iteration, if you call `i` (which has leaked out btw) then it will be equal the result of it's last loop. `let` does not do this.

### Video 04
Temporal dead zone = you cannot access a variable before it has been defined.

### Video 05
when to use `var`/`let`/`const`
Wes and Jason say...
  - use `const` by default
  - only use `let` if rebinding is needed
  - (`var` shouldn't be used)

##Section 02
### Video 06
Arrow functions - 3 main benefits...
  - more concise
  - implicit returns (1 liners easy)
  - doesn't re-bind `this` when you use inside another function (e.g. in click handlers)

- When to use () and when it's unnecessary
- Arrow functions are anonymous functions and so don't leave a very good stack trace.

### Video 07
- implicit return with an object literal

### Video 08
- `this` keyword does NOT get reboud in arrow functions
- 




![ES6 for Everyone](https://es6.io/images/es6-facebook-share.png?cool=yah)
