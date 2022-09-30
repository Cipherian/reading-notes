# Data Structures and Algorithms

What is 1 of the more important things you should consider when deciding which data structure is best suited to solve a particular problem?

- One of the most important things you should consider is the Big O notation, or how long will the operation take. You should consider whether the algorithm will scale with the data that is being input in.

How can we ensure that we’ll avoid an infinite recursive call stack?

- You can avoid an infinite recursive call stack by avoiding having a function call itself without a base case. If you have it invoke itself without letting it know when to stop, it will continue to run until the machine runs out of memory or it is forced to stop.