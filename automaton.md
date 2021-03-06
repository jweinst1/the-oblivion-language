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

Now in classical automaton theory, and formal language theory, only several types of state machines exist. Each one will be demonstrated here, yet keep in mind the Oblivion language implements many richer, more elaborate machines than these.

####Formal Language Theory

Traditionally, automata theory was formulated around the purpose of constructing and reading languages. The mathematical models of finite state machines are closely tied to the linguistic models of grammars, production rules, and language theory. Usually, when one thinks of a machine, or automaton, they think about some *task* being automated or performed. Automaton were originally conceived  to receive textual input, and in doing so, either change it's state according to that input. 

Every classical automaton has some initial state, subsequent states, and it's *final* state. The final state is only entered once the automaton has finished recognizing all the symbols it's needed to. Here is an example.

![](FSA001.png)


This transition diagram of an automaton, or specifically a finite state automaton, shows the progressive recognition of the word `MIT`. At every stage, starting at the initial stage, the machine recognizes one, and only one letter. Once it detects that letter has been seen, it transitions to it's next state. At the final state, it is no longer checking for letters, or awaiting a transition.

#####Alphabets

An alphabet, is some finite set of *symbols*. These symbols, can be concatenated into words, usually called strings in most languages. These symbols, unique from one another, can be combined into strings through some set of rules. The set of all possible strings from some alphabet is called a *formal language*, or language for short. The rules from which strings are constructed from an alphabet is called a *grammar*.

Examples of alphabets:

```
The Binary Alphabet
A = {0, 1}

The Digit Alphabet
A = {-, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9}
```

As long as a non-empty set of finite symbols can be represented, those symbols can be modeled as an alphabet.