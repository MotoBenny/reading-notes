# Read 10

[The JS callstack](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4)

What is a ‘call’?

The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.

How many ‘calls’ can happen at once?

Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.

What does LIFO mean?

last in first out, the last function to get pushed into the stack is the first function to return

Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
``` javascript
function firstFunction(){
  throw new Error('Stack Trace Error');
}

function secondFunction(){
  firstFunction();
}

function thirdFunction(){
  secondFunction();
}

thirdFunction();
// THE RETURN FROM THIS

Uncaught Error: Stack Trace Error
at firstFunction
at secondFunciton
at thirdFunciton
```

What causes a Stack Overflow?

A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accommodate before throwing a stack error.

## Javascript Error Messages

[JS Error Messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

What is a ‘refrence error’?

This is as simple as when you try to use a variable that is not yet declared you get this type os errors.

What is a ‘syntax error’?

his occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

What is a ‘range error’?

Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.

What is a ‘tyep error’?

A tyep error isnt a thing. Its probably a syntax error in of itself.

What is a breakpoint?

It is a point in the code you can add to the console that will cause the program to stop running at that point. A sort of pause. 

What does the word ‘debugger’ do in your code?

It will allow you to see the code history before that point.
