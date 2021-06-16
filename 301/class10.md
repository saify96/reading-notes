## what is a ‘call’?
 - ### The call stack is primarily used for function invocation (call)
 
## How many ‘calls’ can happen at once?
 - ### It is single-threaded. Meaning it can only do one thing at a time.

## what does LIFO mean?
 - ### a LIFO — Last In, First Out data structure.

## Draw an example of a call stack and the functions that would need to be invoked to
 - ### function add(a, b) { return a + b; }

## What causes a Stack Overflow?
 - ### When you call a function in your code, the next instruction after the function call is stored on the stack, and any storage space that might be overwritten by the function call. The function you call might use up more stack for its own local variables. When it's done, it frees up the local variable stack space it used, then returns to the previous function.
---
# ERROR
## WHAT is a ‘refrence error’?
 - ### This is as simple as when you try to use a variable that is not yet declared you get this type os errors.

## WHAT is a ‘syntax error’?
 - ### This occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

## WHAT is a ‘range error’?
 - ### Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.

## WHAT is a ‘tyep error’?
 - ### This types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

## WHAT is a breakpoint?
 - ### If the line you selected was run you will be able to see what has happened before that point and you can try and evaluate the next lines to check if everything is outputting what you are expecting.

