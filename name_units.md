# Name Units

Name Units are structures in Oblivion that are responsible for binding key values that are callable to specific units, patterns, chains, or any value. Name units themselves refer to other units. An important concept is that, you cannot create units by using names to values, you can only refer to them with name units.

The first, lowest level type of name unit is a local. A local binds an alphanumeric name to a type of Unit. Any processes or oper units applied to the named unit all direct toward the unit the name is bound to. Here is an example:

```
{x} -> (6) -> @
@ -> #

~~~ { x=>6 }
```
This Oblivion program binds the local `{x}` to the integer unit `(6)`, and applies that binding to the name space, `@`.