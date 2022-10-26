# Reading Notes 10/22/2022

## Scope

- The concept of scope rules how variables and names are looped up in your code. IT determines the visibility of a variable within the code. The scope of a name or variable depends on the place in your code when you create that variable.

>Global scope: The names that you define in this scope are available to all your code.
>Local scope: The names that you define in this scope are only available or visible to the code within the scope.

- In python the concept of scope is related to the concept of the namespace. Python scope determines where in your program a name is visible. Python scopes are implemented as dicionaries that map names to objects. These dictionaries are called namespaces. They are stored in the modules __dict__ atribute.

- You can find them with:

import sys

sys.__dict__.keys()
dict_keys(['__name__', '__doc__', '__package__',..., 'argv', 'ps1', 'ps2'])

- Python uses the LEGB rule for python scope

> Local (or function) scope is the code block or body of any Python function or lambda expression. This Python scope contains the names that you define inside the function. These names will only be visible from the code of the function. It’s created at function call, not at function definition, so you’ll have as many different local scopes as function calls. This is true even if you call the same function multiple times, or recursively. Each call will result in a new local scope being created.

Enclosing (or nonlocal) scope is a special scope that only exists for nested functions. If the local scope is an inner or nested function, then the enclosing scope is the scope of the outer or enclosing function. This scope contains the names that you define in the enclosing function. The names in the enclosing scope are visible from the code of the inner and enclosing functions.

Global (or module) scope is the top-most scope in a Python program, script, or module. This Python scope contains all of the names that you define at the top level of a program or a module. Names in this Python scope are visible from everywhere in your code.

Built-in scope is a special Python scope that’s created or loaded whenever you run a script or open an interactive session. This scope contains names such as keywords, functions, exceptions, and other attributes that are built into Python. Names in this Python scope are also available from everywhere in your code. It’s automatically loaded by Python when you run a program or script.

- Source: [RealPython](https://realpython.com/python-scope-legb-rule/)
