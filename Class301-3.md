# This is my journal 7/22/2022

## Lists and Keys

> EX: const numbers = [1, 2, 3, 4, 5];
const doubled = numbers.map((number) => number * 2);
console.log(doubled);

- In React, transforming arrays insto lits of elements is similar.

- You can build collections of elements and inlude them in JSX using curly braces {}

- Here's another example where we return an array with an li element.

<!-- > const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li>{number}</li>
); -->

<!-- <ul>{listItems}</ul> -->

- Typically, you render litsts inside ofa component. Here is an example of refactoring the previous example.

<!-- function NumberList(props) {
  const numbers = props.numbers;
  const listItems = numbers.map((number) =>
    <li>{number}</li>
  );
  return (
    <ul>{listItems}</ul>
  );
}

const numbers = [1, 2, 3, 4, 5];
const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(<NumberList numbers={numbers} />); -->

- Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside tthe array.

<!-- > EX: const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li key={number.toString()}>
    {number}
  </li>
); -->

- It's not advised to use indexes for keys if the order of the item may change. This will impact performance and may cause issues with the component state. (robinpokorny.medium.com/index-as-a-key-is-an-anti-pattern-e0349aece318)

> Ex: Correct Key Usage
<!-- function ListItem(props) {
  // Correct! There is no need to specify the key here:
  return <li>{props.value}</li>;
}

function NumberList(props) {
  const numbers = props.numbers;
  const listItems = numbers.map((number) =>
    // Correct! Key should be specified inside the array.
    <ListItem key={number.toString()} value={number} />
  );
  return (
    <ul>
      {listItems}
    </ul>
  ); -->
}

-Keys used within arrays should be unique among their siblings, but don't need to be unique in a global scope. We can use the same keys to produce two different arrays.

> EX: An example of the same key producing different arrays
<!-- function Blog(props) {
  const sidebar = (
    <ul>
      {props.posts.map((post) =>
        <li key={post.id}>
          {post.title}
        </li>
      )}
    </ul>
  );
  const content = props.posts.map((post) =>
    <div key={post.id}>
      <h3>{post.title}</h3>
      <p>{post.content}</p>
    </div>
  );
  return (
    <div>
      {sidebar}
      <hr />
      {content}
    </div>
  );
}

const posts = [
  {id: 1, title: 'Hello World', content: 'Welcome to learning React!'},
  {id: 2, title: 'Installation', content: 'You can install React from npm.'}
];

const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(<Blog posts={posts} />); -->

> An example of map() embeded in JSX
<!-- function NumberList(props) {
  const numbers = props.numbers;
  const listItems = numbers.map((number) =>
    <ListItem key={number.toString()}
              value={number} />
  );
  return (
    <ul>
      {listItems}
    </ul>
  );
} -->

- Sourced: https://reactjs.org/docs/lists-and-keys.html

-In Javascript, spread syntax refers to the use of an ellpsis of three dots to expand something that can be iterated over into a list of arguments.

- Spread was added into ES6, it spreads an array into separate arguments.

>Example: Here are three different math max functions.


Math.max(1,3,5) // 5
Math.max([1,3,5]) // NaN
Math.max(...[1,3,5]) // 5

- The spread operator is a convenient way to copy an array or combine arrays and it can even add new items.

> Example: Copying arrays/Combining and adding new items.

<!-- const fruits = ['🍏','🍊','🍌','🍉','🍍']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "🍏", "🍊", "🍌", "🍉", "🍍" ]
fruits[0] = '🍑'
console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍 -->

- It can also be used to concat arrays.

> Array concatenation:

const myArray = [`🤪`,`🐻`,`🎌`]
const yourArray = [`🙂`,`🤗`,`🤩`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩

- The spread operator can add an item to a list, with natural syntax.

> Ex: Adding to an array
const fewFruit = ['🍏','🍊','🍌']
const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]

- Addning an item to an array in React is easily accomplished in React.

Ex: Adding to an array in React.

> import React, { useState } from "react"
import ReactDOM from "react-dom"

import "./styles.css"

function App() {
  // React Hooks declarations
  const [searches, setSearches] = useState([])
  const [query, setQuery] = useState("")

  const handleClick = () => {
    // Add the search term to the list onClick of Search button
    // (Actually searching would require an API call here)

    // Save search term state to React Hooks
    setSearches(searches => [...searches, query])
  }
  
  // ...

- Source: medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab

- How to pass functions between component?

- You can pass functions as props, which can be passed to objects.