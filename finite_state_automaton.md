# Finite State Automaton

The term *finite* is a little ambiguous when used in the context of computer programming. Everything is essentially, finite in a program. You have a finite amount of memory, for example. However, in the case of automaton, we can take the term "finite" to mean reasonably countable. An `FSA`, for short, has some finite amount of states, in which it can transition from one to another, via an input.

An important distinction in an FSA is whether the automaton is *deterministic* or *non-deterministic*. A deterministic state machine will always have one following or forward state for a specific input. No one input symbol or string can be mapped to more than one state. One state, can be mapped to multiple other states, as long as each transition requires a unique input.

To demonstrate this concept, the model of a baseball field, and the process in which a batter runs across the bases, will be utilized. Let's take a baseball diamond. It has four bases, home, first, second, and third base. First, let's look at this from the perspective of the batter, whom starts the at-bat from home base.

###Baseball Diamond


![](BaseballDiamond.png)

In our model, we want to model the possible states and transition of states that follow the pattern in which the batter runs across the bases. The batter must always start at home base, so that will be the initial state of the automaton.