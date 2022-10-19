# Reading Notes 10/15/2022

## Big O Analysis

- Big O notation is used to describe the efficiency of an algorithm or function. This function is evaluated based on 2 factors

- Running time (The amount of time a function needs to complete)

- Memory Space: the amount of memory resources a function needs to use to store data.

> Big O’s role in algorithm efficiency is to describe the Worst Case of efficiency an algorithm can have in performing it’s job

- Input size refers to the size of the parameter values that are read by the algorithm, this does not simply refer to the number of parameters an alogorithm reads, but takes into account the size of each paramer value as well.

## Units of Measurement

- To evaluate a function for time and space complexity we need the following factors

- The time in milliseconds from the start of a function execution until it ends

- The number of operations that are executed

- The number of basic operations that are executed(refers to the operation that is consuming the most total running time.)

- Memory source is quantified by the following four things:

> The amount of space needed to hold the code for the algorithm.
> Think of this as the number of bytes required to store the characters for >the instructions specified in your function.
> The amount of space needed to hold the input data.
> If direct input data is not considered, we may just refer to this as >Additional Memory Space since not all functions have direct input values.
> The amount of space needed for the output data.
> The amount of space needed to hold working space during the calculation.
> Working Space can be thought of as the creation of variables and reference >points as our function performs calculations. This will also include Stack >Space of recursive function calls … specifically how memory usage scales >relatively with the size of the input.

## Orders of Growth

- The overall efficiency is measured by the input size n 

- Constant complexity means that no matter what inputs are put in the algorithm, it always uses the same time or space.

- Logarithmic complexity represents a function that sees a decrease in the rate of complexity growth, the greater our value of n. This is most often seen when we are performing calculations on sotred data.

- Linear Complexity: The size of our inouts n will directly determine the amount of memory spaceused and running time length. This is a very common efficiency and is usually used to denote functions with loops.

> Linearithmic Complexity:  is used to describe a growth rate of n by lgn. This represents complexity that grows with n, but also by lgn. Linearithmic functions grow faster than input size n, but not by much. This can be seen in divide and conquer algorithms such as the Merge Sort have linearithmic complexity growth rates.
> Quadratic Complexity describes an algorithm with complexity growing at a rate of input size n multiplied by n. This is often seen in algorithms that have nested loops which perform iterative or recursive logic on all values of n and immediately iterate or recurse again for each value of n. Often seen in brute force comparison functions that compare all values of an iterable with each other value.
>Exponential Complexity represents very rapidly growing complexity, such that whatever our input size n, we are performing the same number of iterative or recursive loops as n. If we have to examine subsets of a set of data, and compare against all possible subsets, we may have exponential complexity growth.

## Linked List

- A Data structure that contains nodes that link or point to the next node in the list.

- Singly: Refers to the number of references the node has. A singly linked list means that there is only one reference and the reference points to the next node in a linked list.

- Doubly: refers to there being two double references within the node, they refer to the next and previous node.

- Node: Nodes are individual items that live in a linked list. Each node contains the data for each link.

- Next: Eeach node contains a property called next, it contains the reference to the next node

- Head: The head is a reference type node to the first node in a linked list

- Current: Reference type of node that is currently being looked at, when traversing you create a new curreent variable at the head.

### Traversal

- When traversing a linked list, you are not able to use a foreach or a for loop. We depend on the next value in each ndoe to guide us where the next reference is pointing.

- It is best to use a while loop, this allows use to continually chek that the next node in the list is not null, if we accidentally end up trying to traverse on a node that is null, a NullReferenceException gets thrown and the program will crash.

- Example:
`
  WHILE Current is not NULL
    IF Current.Value is equal to value
      return TRUE

    Current <-- Current.Next

  return FALSE
  `
