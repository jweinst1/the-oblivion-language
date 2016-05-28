# States

A state, in the logical sense, is a singular, identifiable instance of some object or element. An instance, refers to the possession of one or more values, of which two different states will not have the same values. The most common states programming languages feature are `true` and `false`. Typically, a logical expression, such as `5 == 4`, will evaluate to `false`, because it's not valid. 

Both `true` and `false` are different states. `null`, another common state in conventional programming languages, represents the absence of a value. However, it is equally just as much as a state as `true` and `false`. In an abstract sense, we can have many more states than just the Boolean set of `true` and `false`. `A`, `B`, and `C` can, in theory also be thought of as states. We could even think of every word as a state itself. Now, is a number, a state?

####States and Values

Are values and states more or less the same structures? Do they represent the same properties and operations mathematically?

The answer is no, to both questions. A value, such as an integer, is a part of some sequence, where a superior element, and inferior element are present. Such as, the set of all 8-bit unsigned integers that represent bytes. Every member of that set, measures some quantity, relative to other members. Specifically, values have a greater than, `<` or lesser than `>` operations that can be performed on them, while states *do not*. 

The expression `5 > 3` makes sense, as one number can be less than or greater than another number. However, the expression `true > false` is not understandable, and can't be evaluated. Neither `true` nor `false` have quantities of magnitude associated with them, and can't be considered more or less than one another.

#####Logical and Non-Logical Operators

In mathematical logic, logical operations can be applied to one or more states. These operations, always evaluate to some other state, and can only be used on states themselves. The first such operator is the not operator. This appears in programming languages as `not`, such as in Python, or simply `!`, in JavaScript. We will refer to the not operator as `!`.

The `!` operator, when applied to a state, changes the state to it's binary opposite or binary sister state. `!(true)` will change the state to `false`. Conversely, `!(false)` will change the 