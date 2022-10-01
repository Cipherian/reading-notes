# Reading Notes #1 October, 1 2022

## Pain vs Suffering and learning

> All growth comes with some degree of pain, as it pulls you out of your comfort zone. The greater the growth, the greater the pain. But pain in the service of growth is a good thing, as long as that pain is what’s necessary to achieve the growth that you’re aiming for. And even better than that, this pain is only temporary. It’s what will launch you forward into the next phase of your life.

- Suffering is pain without purpose or personal development.

## Big O Notation

- O(1) describes an algorithm that will always executre in the same time regardless of the size of the data that is being put into it.

- O(N) is an algorithm whose performance will grow linearly and in proportion to the size of the data set. Big O notation always assumes the upper limit where an algorithm will perform the maximum number of iterations.

- O(N)^2 represents an algorithm whose performance is directly proportional to the square of the size of the input data set. This is more common with algorithms that involve nested iterations over a data set. Further nested iterations will result in O(N^3), O(N^4) and so on.

-O(2^N) Denotes an algorithm whose growth doubles with each data set that is put into it. This grwoth curve is very exponential, starting shallow and then rising extremely fast.

> EX:
> int Fibonacci(int number)
> {

    if (number <= 1) return number;

    return Fibonacci(number - 2) + Fibonacci(number - 1);

}

## Python Names and Values

- Names refer to values and assignment makes the name refer to the value

- Names are reassigned independently

- Memory is managed dynamically

- Assignment never copies data

- Python has immutable types ints, floats, strings, tuples
