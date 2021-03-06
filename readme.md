# My notes below...

## Section 01
### Video 01
- `var` variables are globally scoped unless inside a function in which they are in "bracket jail" = function scoped but does NOT apply to other brackets (e.g. an `if` statement that is not part of a function).
- `let` and `const` variables are both BLOCK scoped meaning they are scoped to the block (whatever brackets) they are in, including `if` statements or `for` loops.

### Video 02
- Cannot redeclare a `let` variable in the same scope the way you can with `var`
- A `const` variable cannot be changed (as in "constant") but it's properties CAN be updated.
- Although `const` can not be wiped out completely it's properties CAN be changed (if the `const` variable contains an object, the properties of that object CAN be updated). `const` is not immutable.
- If you truly want to lock down a variable use `Object.freeze(potato)`

### Video 03
- an IIFE (Immediately-Invoked Function Expression) is a function that runs before anything else and prevents variables leaking (e.g. `var name = "Wes"` see example in comment - let-const-real-life.html) is not necessary any longer since `let` and `const` are block scoped. Simply put them in brackets.
- in a `for` loop if you use `var i = 0` var is overwritten every time it loops so after the last iteration, if you call `i` (which has leaked out btw) then it will be equal to the result of it's last loop. `let` does not do this.

### Video 04
Temporal dead zone = you cannot access a variable before it has been defined. 🍕🍕🍕

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
- implicit return with an object literal by wrapping the return in parens

### Video 08
- `this` does NOT get rebound to the parent scope with arrow functions - it DOES with standard named functions.
  - e.g. in a click handler on a `<div>` the arrow func is still bound to the window and NOT the parent `<div>`. May be better to use a `function() {do stuff}`

### Video 09 - Default Arguments
- will set default amounts for arguments in functions.
- order matters so if specific arguments are not passed it will return `undefined`
- if you want to skip passing a custom argument when defaults are present, pass `undefined` and will fall back to defaults


![ES6 for Everyone](https://es6.io/images/es6-facebook-share.png?cool=yah)
