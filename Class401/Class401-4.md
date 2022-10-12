# Reading Notes 10/11/2022

## Classes and objects

> Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. Classes are essentially a template to create your objects.
> You can create multiple different objects that are of the same class(have the same variables and functions defined). However, each object contains independent copies of the variables defined in the class. For instance, if we were to define another object with the "MyClass" class and then change the string in the variable above:

- An example of using class:

`class MyClass:
variable = "blah"

    def function(self):
        print("This is a message inside the class.")

myobjectx = MyClass()

myobjectx.function()`

- The \__init_() function is a special function that is called when the class is being initiated.

## Thinking recursively

- An example of a recursive function

`

- houses = ["Eric's house", "Kenny's house", "Kyle's house", "Stan's house"]

- Each function call represents an elf doing his work

def deliver_presents_recursively(houses): # Worker elf doing his work
if len(houses) == 1:
house = houses[0]
print("Delivering presents to", house)

    # Manager elf doing his work
    else:
        mid = len(houses) // 2
        first_half = houses[:mid]
        second_half = houses[mid:]

        # Divides his work among two elves
        deliver_presents_recursively(first_half)
        deliver_presents_recursively(second_half)`

- Now that we have some intuition about recursion, let’s introduce the formal definition of a recursive function. A recursive function is a function defined in terms of itself via self-referential expressions.

- This means that the function will continue to call itself and repeat its behavior until some condition is met to return a result. All recursive functions share a common structure made up of two parts: base case and recursive case.

- Behind the scenes, each recursive call adds a stack frame (containing its execution context) to the call stack until we reach the base case. Then, the stack begins to unwind as each call returns its results:

- Source: [RealPython](https://realpython.com/python-thinking-recursively/)
- Source: [LearnPython](https://www.learnpython.org/en/Classes_and_Objects)
