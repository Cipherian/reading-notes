# Reading Notes 10/8/2022

## What is a file?

- Header: metadata about the contents of the file (file name, size, type, and so on)

- Data: contents of the file as written by the creator or editor

- End of file (EOF): special character that indicates the end of the file

- When you access a file on an operating system a file path is required

## Python file manipulation

- When you want to work with a file in Python, you need to utilize the .open method.

- You should always make sure an open file is closed properly.

- Leaving a file can lead to unwanted behavior like resource leaks. When you're changing a file there are two ways you can make sure a file closes.

- One is the try finally block.

- `try { file processing goes here } finally { reader.close() }`

- The second method is the "with" statement automatically takes care of closing the file once it leaves the with block.

- with open('dog_breeds.txt', 'r') as reader:
    <!-- # Further file processing goes here -->

- The three different categories of file types are text files, buffered binary and raw file types.

- Text example: `open('abc.txt', 'rb')`

- Buffered binary example: `open('abc.txt', 'rb', buffering=0)`

- Raw file example: `open('abc.txt', 'rb', buffering=0)` (Not commonly used)

## Reading and writing opened files

> .read(size=-1): This reads from the file based on the number of size bytes. If no argument is passed or None or -1 is passed, then the entire file is read.
> .readline(size=-1): This reads at most size number of characters from the line. This continues to the end of the line and then wraps back around. If no argument is passed or None or -1 is passed, then the entire line (or rest of the line) is read.
> .readlines(): This reads the remaining lines from the file object and returns them as a list.

## Exceptions versus Syntax Errors

- Syntax errors: They occur when the parser detects an incorrect statement. Observe the following example:

`>>> print( 0 / 0 )) File "<stdin>", line 1 print( 0 / 0 )) ^ SyntaxError: invalid syntax`

- The arrow shows the extra bracket.

- raise Exception can be used to throw an exception when a condition occurs.

- `x = 10 if x > 5:
  raise Exception('x should not exceed 5. The value of x was: {}'.format(x))`

- This will output:

> `Traceback (most recent call last):
    File "<input>", line 4, in <module>
  Exception: x should not exceed 5. The value of x was: 10`

## The AssertionError Exception

- Instead of waiting for a program to crash midway, you can also start by making an assertion in python. We assert that a certain condition is met and if this condion is met and turns out to be true the program will continue running. If this condition turns out to be false, then the program will throw an assertionerror exception

> Ex:
  import sys
  assert ('linux' in sys.platform), "This code runs on Linux only."

- On windows this would give the error:

> `Traceback (most recent call last):
  File "<input>", line 2, in <module>
  AssertionError: This code runs on Linux only.`

Source 1: [Real Python exceptions](https://realpython.com/python-exceptions/)
Source 2: [Real Python read and write files](https://realpython.com/read-write-files-python/)



