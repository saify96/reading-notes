# Primitives vs. Objects

## Java Data Types are divided into two groups:
   - A primitive
   - Non-Primitive (reference types) because they refer to objects.
- Wrapper classes provide a way to use primitive data types (int, boolean, etc..) as objects.
- The process of converting a primitive type to a reference one is called autoboxing, the opposite process is called unboxing.
- When we decide to use primative types as objects we should consider what application performance we try to achieve, how much available memory we have.
- The reference types are objects, they live on the heap and are relatively slow to access. 

## Performance

- The performance of a Java code is quite a subtle issue, it depends very much on the hardware on which the code runs, on the compiler that might perform certain optimizations, on the state of the virtual machine, on the activity of other processes in the operating system.
- primitive types live in the stack while the reference types live in the heap.
- it's required more time to perform the operation for wrapper classes.

## Default Values

-  Default values of the primitive types are 0 for numeric types.
 false for the boolean type
 \u0000 for the char type.
 For the wrapper classes, the default value is null
 
## Exceptions

- An exception is an event, which occurs during the execution of a program, that disrupts the normal flow of the program's instructions
- When an error occurs, Java will normally stop and generate an error message. The technical term for this is: Java will throw an exception (throw an error).

- Creating an exception object and handing it to the runtime system is called throwing an exception.
### Three Kinds of Exceptions

- The first kind of exception is the checked exception
- The second kind of exception is the error
- The third kind of exception is the runtime exception
- Any code can throw an exception
- All methods use the throw statement to throw an exception.
- Most programs throw and catch objects that derive from the Exception class

## Java try and catch

- The try statement allows you to define a block of code to be tested for errors while it is being executed.
- The catch statement allows you to define a block of code to be executed, if an error occurs in the try block.

## The try-with-resources Statement
- The try-with-resources statement ensures that each resource is closed at the end of the statement.

## Advantages of Exceptions
- Separating Error-Handling Code from "Regular" Code
- Propagating Errors Up the Call Stack
- Grouping and Differentiating Error Types

## Scanning
- Objects of type Scanner are useful for breaking down formatted input into tokens and translating individual tokens according to their data type.
- The Scanner class is used to get user input, and it is found in the java.util package.








