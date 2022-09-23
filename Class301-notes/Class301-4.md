# This is my journal 7/26/2022

## What is a ‘Controlled Component’?

> In HTML, form elements such as input, textarea, and select typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().

> Specifying the value prop on a controlled component prevents the user from changing the input unless you desire so. If you’ve specified a value but the input is still editable, you may have accidentally set value to undefined or null.

- In React, a textarea uses a value attribute instead. This way, a form using a textarea can be written very similarly to a form that uses a single-line input:

- In HTML, select creates a drop-down list. For example, this HTML creates a drop-down list of flavors:

## How do we target what the user is entering if we have an event handler on an input field?

- onChange and value

## Why would we use a ternary operator?

- Using a conditional, like an if statement, allows us to specify that a certain block of code should be executed if a certain condition is met.

## Rewrite the following statement using a ternary statement:

- (x===y) ? console.log(true): console.log(false);
