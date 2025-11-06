---
tags:
  - technique
  - datatype
  - terminology
---

LAMBDA UDTs use [[LAMBDA]] to define custom data types that emulate the [object-oriented programming paradigm](https://en.wikipedia.org/wiki/Object-oriented_programming).

A *user-defined type* (UDT) combines [fields](https://en.wikipedia.org/wiki/Field_(computer_science)) and [methods](https://en.wikipedia.org/wiki/Method_(computer_programming)) into a structured [[term]].

### Overview

LAMBDA UDTs follow the general form:

```gse
lambda(i, choose(i, a, b, ...))
```

Data is [encapsulated](https://en.wikipedia.org/wiki/Encapsulation_(computer_programming)) inside a number of user-defined fields, listed as `a,b...` in the expression above.

These fields can contain any [[term]] except for [[Term#Primitive function|primitives]].

In essence, LAMBDA UDTs allow users to define composite data structures that can serve as both inputs and outputs for user-defined functions.

### Instantiation

UDTs must be [instantiated](https://en.wikipedia.org/wiki/Instance_(computer_science)) with specific field values before they can be used.

They can be instantiated manually or via a constructor pattern:

```gse
=let(
    udt,lambda(a,b...,
        lambda(i,choose(i,a,b...))
    ),
    udt(a,b...)
)
```

The expression above creates an instance of the type `udt`.
Note that the resulting value is a lambda term; it cannot be directly displayed in a cell.

### Field access

To access a stored field, provide an index argument to the instantiated term:

```gse
=let(
    udt,lambda(a,b...,
        lambda(i,choose(i,a,b...))
    ),
    udt(a,b...)(<index>)
)
```

This applies the index via [β-reduction](https://en.wikipedia.org/wiki/Lambda_calculus#%CE%B2-reduction_2), returning the field corresponding to that index.

### Notes
- [[Calculation limits]] represent a major limitation to LAMBDA UDTs, as they are heavily LAMBDA-intensive in nature and can quickly hit the recursion limit.

### See Also

#### Lists

- [Singly-Linked List](https://docs.google.com/spreadsheets/d/1NCpS9HH_IOQGtYby1qE1h7F5WqvuGFlNiPfXh_zMHFQ/edit?gid=0#gid=0)
- [Doubly-Linked List](https://docs.google.com/spreadsheets/d/1JPlLJjkWFH40drkoQFJsMggoaNqqjdAGyQbxbN3YlP8/edit?gid=0#gid=0)
- [SX by Shay](https://docs.google.com/spreadsheets/d/1a-XZAvGKkyKz-XImfmxemYcAQqhpgq3aLXQa1SMk1-0/edit?gid=1778054978#gid=1778054978)

#### Trees

- [Binary Search Tree](https://docs.google.com/spreadsheets/d/1o4KlsxVrp-ylj3juHKPtLaMJS2xF-CNwkeREYrWd4Jg/edit?gid=0#gid=0)
