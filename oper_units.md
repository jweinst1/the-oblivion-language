# Oper Units

Oper units are units that do not contain any referable values, but instead contain an operation. This means that, they carry a potential value that is applied to another unit. They also use arrow brackets, `<>` instead of the parenthesis `()`. For example, if the unit `( 3 )` refers to the integer value of 3, the oper unit `< +3 >` refers to the operation of adding 3. As a result, an oper unit must have a type of `V-Unit` being applied toward it.

####Implementation and availability

In traditional languages, objects and reference types normally have specific methods defined for them. If an object does not carry a particular method, that method cannot be used on an instance of the object. Methods, are a flexible, user-written portion of the language, while an operator is static and unchangeable.

Oblivion seeks to break this barrier, by allowing oper units to be utilized as methods to invoke on specific units. An Oper, has one, abstract purpose, which is customized to individual uses for different units and objects.

For example, the `<+>` oper, has an abstract purpose of adding or concatenation, between a unit and the value associated with it. For `I-Units`, the specific purpose is to add two numbers together. For a string unit, the purpose is to concatenate them into one string. Here is an example:

```
I-Unit 
(6) -> <+3> -> #
~~~ 9

S-Unit
("Flowers") -> <+3> -> #
~~~ "Flowers3"
```