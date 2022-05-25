# This is my journal 5/24/2022

## What I have learned today

> If Javascript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handling code. 

- You can use a set of statements to handle the error. If the script is not handled the script will stop going.

- Error objects contain type of error, description, name of JS file, line number error

- built in error objects contain error, syntax error, reference error, type error, range error, URI error, eval error

- syntax error is incorrect use of the rules of the language, often caused by a typo

- reference error is caused by a variable or out of scope.

- type error is caused by using object or method that doesn't exist

- Range error if you call a function using numbers outside its accepted range

- debug the script to fix errors, track down the source of the code to fix it

- Handle errors as gracefully as possible. Make sure to use try, catch, throw and finally statements.

- Chrome and opera have free debugging tools

- Using more than one browser can help because they will show different errors.

- It is important to console.log in order to find values so you know where the issue is.

-Using the console assert method or console.assert, you can test if a condition is met.