# This is my journal 7/30/2022

## What is the single responsibility principle and how does it apply to components?

- A component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.

## What does it mean to build a ‘static’ version of your application?

- Static means to reuse other components and pass data using props, don't use state at all.

## Once you have a static application, what do you need to add?

- You will need state in order to make your application responsive.

## What are the three questions you can ask to determine if something is state?

> Is it passed in from a parent via props? If so, it probably isn’t state.
Does it remain unchanged over time? If so, it probably isn’t state.
Can you compute it based on any other state or props in your component? If so, it isn’t state.

## How can you identify where state needs to live?

- Find the common parent component that controls the child components and if there is no common parent component, create one.

## What is a “higher-order function”?

- Functions that operate on other functions, either by taking them as arguments or by returning them, are called higher-order functions.

## Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

- It returns the value of m when it is greater than the value of n, which in the case given is greater than 10.

## Explain how either map or reduce operates, with regards to higher-order functions.

> Higher-order functions start to shine when you need to compose operations. As an example, let’s write code that finds the average year of origin for living and dead scripts in the data set.

- They increase readability, as well as increase convenience.

- Sources: (reactjs.org/docs/thinking-in-react.html) (eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)