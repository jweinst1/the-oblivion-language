# States

A state, in the logical sense, is a singular, identifiable instance of some object or element. An instance, refers to the possession of one or more values, of which two different states will not have the same values. The most common states programming languages feature are `true` and `false`. Typically, a logical expression, such as `5 == 4`, will evaluate to `false`, because it's not valid. 

Both `true` and `false` are different states. `null`, another common state in conventional programming languages, represents the absence of a value. However, it is equally just as much as a state as `true` and `false`. In an abstract sense, we can have many more states than just the Boolean set of `true` and `false`. `A`, `B`, and `C` can, in theory also be thought of as states. We could even think of every word as a state itself. Now, is a number, a state?

####States and Values

Are values and states more or less the same structures? Do they represent the same properties and operations mathematically?

The answer is no, to both questions. A value, such as an integer, is a part of some sequence, where a superior element, and inferior element are present. Such as, the set of all 8-bit unsigned integers that represent bytes. Every member of that set, measures some quantity, relative to other members. Specifically, values have a greater than, `<` or lesser than `>` operations that can be performed on them, while states *do not*. 

The expression `5 > 3` makes sense, as one number can be less than or greater than another number. However, the expression `true > false` is not understandable, and can't be evaluated. Neither `true` nor `false` have quantities of magnitude associated with them, and can't be considered more or less than one another.

#####Logical Operators

In mathematical logic, logical operations can be applied to one or more states. These operations, always evaluate to some other state, and can only be used on states themselves. The first such operator is the not operator. This appears in programming languages as `not`, such as in Python, or simply `!`, in JavaScript. We will refer to the not operator as `!`.

The `!` operator, when applied to a state, changes the state to it's binary opposite or binary sister state. `!(true)` will change the state to `false`. Conversely, `!(false)` will change the state to `true`. Not all states however, have a *specific* binary opposite. The `!` operator can also refer to a range of of other states. 

The expression `!(null)`, refers to a state which is not `null`. It can be `true`, `false`, `None`, or a number of other states. However, the question might arise, can the not operator be applied to a value? It most certainly can be, yet this does not yield a value, yet a state. If we take the state `!(1)`, we can think of this as a state of not *being* 1. Any other occurrence can take place, just not `1`. 

Next is the *and* operator, usually denoted via a `&&` in most languages, or in mathematics as $$^$$. The *and* operator is applied to one or more state operands, to determine if both operands have, or evaluate to the same state. The *and* operator will evaluate to the `true` state if every single one of the operands are the same state, or false if any element is a different state.

For example,



```
5 == 5 && 3 > 5

```

This expression will evaluate to false, as the right operand is false, a different state from the left operand, which refers to the true state. *Note: The Oblivion language enables such expressions to result in more than true or false states*.

The *or* operator is similar to the *and* operator, denoted by a `||` symbol in most languages. It evaluates two or more operands, determining if any of the states evaluates to the `true` state. The operator can be chained, such that from left to right, every state is determined if it corresponds to being true. The following expression,

```
5 > 7 || false || 5 == 5
```

will evaluate to true, because the right most operand is true.

In general, logical operations can take both values and states as operands, yet they will always result in a state, not a value. 

#####Non-logical Operators

Another point of difference between values and states are other binary operators, such as arithmetic operators, `+`, `-`, `*`, and more. These listed often represent addition, subtraction, and multiplication. When we apply values, such as a number, to an artihmetic operator, the result is always a new number. Or as in programming, if one concatenates two strings,

```
 >>> "hello" + " " + "world!"
 "hello world!"
```

You get a new string, different from all the operands, returned to you. 

States do not have the ability to generate unique, new states from arithmetic operators. They can only really be expressed in different ways, yet they can never evaluate to other states from using these operators. 

Now that the differences between states and values has been discussed, the mechanics of automaton, or state machines, can be explained.