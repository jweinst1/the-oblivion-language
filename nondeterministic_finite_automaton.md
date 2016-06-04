# Non-deterministic Finite Automaton


The defining, most significant rule that must be followed by a *deterministic* finite automaton is that for every instruction or input, there is always on and only one corresponding transition. Whenever this rule is broken, a machine become *Non-deterministic*, meaning that an instruction is no longer entirely deterministic of it's next state.

For short, an `NFA` allows an input to transition to two or more possible states. Following the earlier example of a baseball game, an `NFA` would exist as a model for the game if a batter were allowed to run to first *or* third base after successfully batting the ball.

Classically, however, the `NFA` model was conceived to allow the interpretation of context-sensitive languages, and most commonly regular expressions. This chapter will present a more tangible, real world example of an `NFA`, before going over regular languages and their capabilities.

