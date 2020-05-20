# Read: 10 - JS Debugging

## Error Handling & Debugging
> JavaScript can be hard to learn and everyone makes
mistakes when writing it. This chapter will help you learn
how to find the errors in your code. It will also teach you how
to write scripts that deal with potential errors gracefully.

**order of execution (the order in which statements are processed)**
* `function greetUser () {`
*  `return 'He11o ' + getName ();`
* `function getName() {`
* `var name= 'Molly ' ;`
* `return name;`
* `var greeting= greetUser();`  
* `alert(greeting);`

 * The greeting variable gets its value from the
greetUser() function.
* greetUser() creates the message by combining
the string 'He11o ' with the result of getName ().
* getName () returns the name to greetUser() .
* greetUser() now knows the name, and combines
it with the string. It then returns the message to the
statement that ca lled it in step 1.
* The va lue of the greeting is stored in memory.
* This greeting variable is written to an alert box.


## Errors Types:

Error    |  Description
---------|---------
EvalError  |  Raised when the eval() functions is used in an incorrect manner.	
RangeError   |  Raised when a numeric variable exceeds its allowed range.
ReferenceError   |  Raised when an invalid reference is used.	
SyntaxError     | Raised when a syntax error occurs while parsing JavaScript code.	
TypeError  |  Raised when the type of a variable is not as expected.
URIError  |  Raised when the encodeURI() or decodeURI() functions are used in an incorrect manner.



**Summary**

* If you understand execution contexts (which have two
stages) and stacks, you are more likely to find the error
in your code.
* Debugging is the process of finding errors. It involves a
process of deduction.
* The console helps narrow down the area in which the
error is located, so you can try to find the exact error.
* JavaScript has 7 different types of errors. Each creates
its own error object, which can tell you its line number
and gives a description of the error.
* If you know that you may get an error, you can handle
it gracefully using the try, catch, finally statements.
Use them to give your users helpful feedback.
