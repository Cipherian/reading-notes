# This is my journal 8/13/2022

## What is functional programming?

- Functional programing is the programming paradigm which aims to compute and do math evaluations and not chage state or muteable data.

## What is a pure function and how do we know if something is a pure function?

> It returns the same result if given the same arguments (it is also referred as deterministic)

It does not cause any observable side effects.

## What are the benefits of a pure function?

- It tends avoids any observable side effects. Code is easier to test and we can easily test pure functions with different contexts or parameters.

## What is immutability?

- When data is immutable, its state cannot change after it’s created.

## What is Referential transparency?

- Pure functions and immutability together make up referential transparency.

## What is a module?

- Code blocks that are split up and have a specific functionality so they can be called when needed.

## What does the word ‘require’ do?

- Require looks for what's exported in another file, which allows you to use variables or functions declared in another file.

## How do we bring another module into the file the we are working in?

- With Export from that file and require in the file you are working in.

## What do we have to do to make a module available?

- Export.