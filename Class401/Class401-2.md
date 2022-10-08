# Reading Notes 10/4/2022

## Unit Tests

> Unit tests are some pieces of code to exercise the input, the output and the behaviour of your code. You can write them anytime you want.

- Test driven development is a strategy and method to write tests first

## AAA

- Arrange: you need to organize the data needed to execute that piece of code (input);

- Act: here you will execute the code being tested (exercise the behaviour);

- Assert: after executing the code, you will check if the result (output) is the same as you were expecting.

## The Cycle

> 🆘 Write a unit test and make it fail (it needs to fail because the feature isn’t there, right? If this test passes, call the Ghostbusters, really)
> ✅ Write the feature and make the test pass! (you can dance after that)
> 🔵 Refactor the code — the first version doesn’t need to be the beautiful one (don’t be shy)

- Source: [codelikeagirl](code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932)

## If __name__ = __main__

- Before executing code, Python interpreter reads source file and define few special variables/global variables.

> If the python interpreter is running that module (the source file) as the main program, it sets the special __name__ variable to have a value “__main__”. If this file is being imported from another module, __name__ will be set to the module’s name. Module’s name is available as value to __name__ global variable.

- A module is a file containing Python definitions and statements. The file name is the module name with the suffix .py appended.

## Advantages

- Every Python module has it’s __name__ defined and if this is ‘__main__’, it implies that the module is being run standalone by the user and we can do corresponding appropriate actions.

- If you import this script as a module in another script, the __name__ is set to the name of the script/module.

- Python files can act as either reusable modules, or as standalone programs.

- If __name__ == “main”: is used to execute some code only if the file was run directly, and not imported.

- Source: [GFG](https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/)

## Recursion

- When a function calls itself directly or indirectly is called recursion

- Recursion is an amazing technique with the help of which we can reduce the length of our code and make it easier to read and write.

## Properties of Recursion

- Performing the same operations multiple times with different inputs.

- In every step, we try smaller inputs to make the problem smaller.

- Base condition is needed to stop the recursion otherwise infinite loop will occur.

## Mathmatical Interpretation

- f(n) = 1 + 2 + 3 +……..+ n

