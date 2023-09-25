## Changing the State of a Data Structure using Functional Programming


Changing the State of a Data Structure using Functional Programming
In purely functional programming, we typically avoid changing the state of data structures. Instead, we create new instances or objects with modified values, ensuring immutability. For example, if you have a list and want to "modify" it by adding an element, you'd create a new list with the additional element rather than modifying the original list in-place.

## Purely Functional Programming

Purely functional programming consists of ensuring that functions, inside the functional paradigm, will only depend on their arguments, regardless of any global or local state. A pure functional subroutine only has visibility of changes of state represented by state variables included in its scope.


## How do you think purely functional programming will differ from the programs you’ve written so far in this course?

- Purely functional programs are more declarative, while imperative programs are more procedural. Declarative programming focuses on describing the desired outcome of a computation, while procedural programming focuses on specifying the steps that the computer must take to achieve that outcome.
- Purely functional programs avoid side effects, while imperative programs often rely on them. A side effect is any change to the state of the program outside of the function that is currently being executed. Purely functional programs are more predictable and easier to reason about because they avoid side effects.
- Purely functional programs use immutable data structures, while imperative programs typically use mutable data structures. Immutable data structures cannot be changed once they are created. This makes purely functional programs more thread-safe and easier to parallelize.
