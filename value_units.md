# Value Units

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