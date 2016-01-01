# Chapter One: Units

Units are the most basic component of any code written in Oblivion. They are small, simple elements that each have a single purpose and function. The concept behind this is that, the composition of units in a Oblivion program is highly flexible in it's style and layout. One goal can be achieved in many different ways.

## Value Units

The first fundamental type of unit in Oblivion is the value unit, also called a `V-Unit`. A V-Unit represents a reference, or pointer to a specific value, or in some cases an object. A V-Unit, in the simplest sense, cannot do anything in and of itself. This type of unit can only have other units applied to it, or have itself applied to other units.

#### Integer Unit

An Integer Unit, also called a `I-Unit`, contains a single integer value:

```
(5)
(7)
(999)
(-88)
```
#### String Units

A String Unit, also called an `S-Unit`, contains a series of string characters. These units work differently than other languages. There is no empty string unit, all strings must have at least one character in them. Additionally, S-Unit's are also mutable, and thus act as an ordered collection. This will be covered in further chapters. Here are some examples:

```
("sir")
("yes")
("The Oblivion Language")
```
#### Double Units

A Double Unit, is a unit that contains a single floating point number, such as `1.27`.

```
(9.8875)
(334.67)
```

#### Bool Units

A Bool Unit, also called a `B-Unit`, is a value unit that contains either the value `true` or `false`.

```
(true)
(false)
```



##Oper Units

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

####Arithmetic Opers

Arithmetic Opers have basic, abstract purposes, and can be used in a variety of ways. They all operate in a single step, and thus can be compounded to create much larger processes. Arithmetic opers can be repeatedly applied in the same unit, by repeating their operator sign.

```
(9) -> <*3> -> #
~~~ 27

(9) -> <+++3> -> #
~~~ 18
```

#####Plus Oper

The plus oper, `<+>`, is responsible 