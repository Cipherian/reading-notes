# Reading Notes 10/25/2022

## List comprehnsion

- There are three ingredients necessary for python list comprehension to work.

> First is the expression we’d like to carry out. expression inside the square brackets.
> Second is the object that the expression will work on. item inside the square brackets.
> Finally, we need an iterable list of objects to build our new list from. list inside the square brackets.

- You can perform expressions on an entire list in a single line of code, we can also add conditional statements with filters, which allows for more precision in the way lists are handled

- Notes:

> List comprehension methods are an elegant way to create and manage lists. 
> In Python, list comprehensions are a more compact way of creating lists. 
> More flexible than for loops, list comprehension is usually faster than other methods.

- Create a list with range() and pass in a number to create a list with numbers

- `for i in range(10)` creates a list [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

- Extract digits from a string with "isdigit method.

```Example:
user_data = "Elvis Presley 987-654-3210"
phone_number = [ x for x in user_data if x.isdigit()]
print(phone_number)
```
