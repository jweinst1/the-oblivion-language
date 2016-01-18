# Chapter Two: Connectors

In Oblivion, every unit is related to another unit by a connector. Connectors employ the task of mapping one unit to another, and compounding the successive mapping of several units into more units. They are perhaps the most abstract feature in all Oblivion, since they allow very low level processing and flexibility. The concept of connectors is to completely undo the standard features of a programming language, such as for loops, functions, classes, exceptions, as well as instances, and give way for a genuine new experience. Here is a formal definition of a connector:

> A Connector is a symbolic element that represents a relationship between two or more units. It is responsible for embodying meaning between units, and how they will carry out a process.

Every series of Units and Connectors only concerns a single, linear process. This means that, units are linked together in one stream. You can only access another binding or unit if you start use the `|` terminator. The placing of Oblivion statements is very flexible, so you can make a single program into a single line, or many lines if you wish.

All connectors have some indication of direction, or the order in which units are related to one another. This is very important, because all processes need to have a clear starting and ending point. For example, `(6) -> <+3>` uses the right applicator connector, or `RAC` for short. This takes the left unit and applies it to the right unit. In contrast, `(6) <- <+3>` takes the right hand unit and applies it to the left hand unit, also called `LAC` for short. In the example, `<+3>` becomes `<+9>`.

Now, at first glance, the applicators discussed above seem identical to each other, one just offering a "cool" variation of code being read backwards. However, when both the left hand and right hand applicators are used together, we can produce some very interesting effects.

```
(8) -> # <- (7)
~~~ 8
~~~ 7
```

The above process is equivalent to `(8) -> #: (7) -> #`. The applicator units can also be implemented with opposite directions. 

```
# <- (8) -> #
~~~ 8
~~~ 8
```

The applicators, along with many of the other connectors, can be abstracted in an incredible number of ways to produce a highly custom feature of the Oblivion language.
