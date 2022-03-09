Class-10.md

## **Table Of Contents**

_Read:_ 10 - Forms and Events


## ***Ducket js***

1. JavaScript book, Ch. 10, “Error Handling & Debugging”

## ***Ducket js***

### **Error Handling & Debugging**

- the first step in debugging code is completely understanding the order of execution
- an error in JS will contain the following properties
- `name` the type of execution `message` description `filenumber` name of JS file `lineNumber` line of error.
- `syntax error` incorrect use of rules of JS > often as simple as a typo in the code
- `reference error` variable not declared or out of scope
- `type error` caused by trying to use an object or method that does not exsist
- `range error` if you call a function with numbers outside its accepted range
- `EvalError` evaluates text through the interpreter < you will rarely if ever see this>
- `URI Error` incorrect use of URI functions (incorrect use of escape characters)
- `Error` generic error object
- `NaN` Not a number error

# debugging workflow

1. Where is the problem?
  - location the relevant script and read through it, see how far it runs thorough the code.

2. What exactly is the problem (what is the error type?)
  - find the actual line of code the error is on, Check values of any arguments passed to that line

- anytime something is wrong, console.log all the things. Any values or parameters handed to that function or code.
- write smart logs that tell you where in the code you are.
- console.table() will help when logging objects or arrays
- console.assert() allows you to test if a condition is met.
- try, catch, finally to handle exceptions 
- if you suspect a problem area of your code, you can generate your own errors before the interpreter `throw new Error(message)`
