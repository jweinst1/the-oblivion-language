# Automaton

When someone thinks about machines, they often think about factories, robots, engines, and gears. Factories, are composed of specific machines that automate various tasks. Each machine, is often operated via changing it's mode of function, or mode of operation. When a car goes from park, to drive, to reverse, the car is changing its *states* of motion.

Now, how does the car change it's state of motion? It receives input from the driver, through a lever, or a stick shift. Every change in the positioning of a stick shift changes the *input* being received by the car. The inputs determine the state which the car drives in. Changing the input changes the state.

####The Light Switch

The simplest machine, in abstract terms, is a light switch. A light switch, one that can be turned on and off. When the switch is pointing up, the light is on. When the switch is pointing down, the light is off. The light switch's input instructions, `up` or `down`, determine it's state, `on` or `off`. We can construct a state diagram, mapping out the states and transitions of a simple light switch.

![](Untitled Diagram.png)

The arrows pointing back toward their own box indicate an *unaccepted* input. Flipping a switch up when it is already pointing up and on won't do anything. This works the same for flipping the switch down when the switch is already pointing down.

A light switch, therefore, has a set of two states, on and off, with two possible inputs, up and down. Here is a pseudo-code representation of this machine.

```
switch = (
    states:{on, off}
    inputs:{up, down}
)
```

Mathematically, automaton are defined as moving from one state to another via a *transition function*. The Oblivion language, however, does not use functions or function objects. This portion of automaton theory will be left out, until it can be explained in terms of Oblivion's machinery.