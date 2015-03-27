# Aspenware Engineering Manifesto

This document sets forth the principles by which Aspenware engineers go about
writing software for our clients. It is broadly organized into several core
values that each go into detail on what they are, why they're important to us,
and the implications of using them.

This is a collaborative document. All Aspenware engineers have a say in its
content. Propose changes to this document by pull request. Changes are adopted
by consensus.

## Justification

TODO Mike put your thoughts here

## Terminology

Aspenware leverages several programming languages and technologies to achieve
its goals, and these all have different ways to refer to the same set of ideas.
To reduce ambiguity, we have set forth a few terms that are used in this
document:

**Types** are a language construct that define the schema of a kind of data, and
in some languages also defines the ways in which that data may be manipulated.

A **function** is a way of encapsulating logic. It is the implementation of the
ways in which data is manipulated.

A **contract** is an explicitly defined set of behaviors that support certain
goals within a broader application. An **implementation** fulfills this
contract.

An **abstraction** is a mechanism through which the details of a particular
procedure are hidden. Through abstractions, the solution to a problem is defined
in terms of "what it does, rather than how it does it".

## 1: Maintainability

We strive to write code that is transparent in its intent. We recognize the
software we write is inherited by other developers and in doing so we have a
responsibility to design and implement our software in such a way that it can be
carried forward to use-cases that we never envisioned.

### 1.1: Maintainable code

We prefer code that is structured in a way that explains itself to a reader
experienced in the language over code that uses comments to explain its logic.
That's not to say that comments are not welcome in our code - we instead prefer
comments that justify the reasoning behind the code, or comments that describe
the broader purpose of the code.

This can be accomplished by using variable and function names that are clear and
meaningful, and by splitting up complex logic into several discrete functions.
Do not depend on behavior specific to one implementation of a contract - if the
contract does not satisfy the requirements, alter the contract.

### 1.2: Maintainable architecture

A maintainable architecture enables the developer to understand and extend the
broader application. We do not value a monolithic architecture - instead, we
write modular components and compose them to solve our problems.

### 1.3: SOLID

At Aspenware, we observe the SOLID principles, reproduced here:

**S**ingle responsibility - a type should solve a single problem.

**O**pen/closed - types should be open for extension, but closed for
modification.

**L**iskov substitution - types should be replacable with instances of their
subtypes without altering the correctness of the program.

**I**nterface segregation - many client-specific interfaces are better than one
general-purpose interface.

**D**ependency inversion - one should depend upon abstractions. Do not depend on
implementations.

## 2: Elegance

[todo: wavy hands, hack value]

## 3: Ethical Software Development

[todo: things like security, responsible disclosure, things we don't do for our
clients, maintaining the value of our profession]

## 4: 
