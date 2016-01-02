The Oblivion Language
=======

Oblivion is a modern programming language that takes an unorthodox approach to syntax and computing. The concept of syntactic sugar is heavily emphasized, making the code readable in a linear, step by step fashion. Oblivion uses many different basic concepts, with the ideology that smaller, simple pieces of code can be more easily abstracted into larger, more sophisticated programs.

Oblivion is structured around the concept units. Instead of having defined, built in statements, the language composes all statements from series of operations. For example, `x = 1`, from Python, binds the variable `x` to the integer 1. Or in Java, one would write `int x = 1`.

In Oblivion, the proper expression to match a simple assignment is `{x} -> (6) -> @`. Here, we perform the assignment via a stream of units. The `{x}` expression is called a name unit, which is similar to the concept of a parameter in other languages. The `->` expression is the apply unit. This takes the previous unit and applies it to the next unit. The `@` symbol represents the bindings unit. It is similar to a local and global bindings scheme in languages like Python.

For more information, see the [manual.](SUMMARY.md)

For the Java Implementation of Oblivion, click [here](https://github.com/jweinst1/Oblivion-Java)

For the JavaScript/Typescript implementation of Oblivion, click [here](https://github.com/jweinst1/OblivionJS)

