# Finite State Automaton

The term *finite* is a little ambiguous when used in the context of computer programming. Everything is essentially, finite in a program. You have a finite amount of memory, for example. However, in the case of automaton, we can take the term "finite" to mean reasonably countable. An `FSA`, for short, has some finite amount of states, in which it can transition from one to another, via an input.

An important distinction in an FSA is whether the automaton is *deterministic* or *non-deterministic*. A deterministic state machine will always have one following or forward state for a specific input. No one input symbol or string can be mapped to more than one state. One state, can be mapped to multiple other states, as long as each transition requires a unique input.

To demonstrate this concept, the model of a baseball field, and the process in which a batter runs across the bases, will be utilized. Let's take a baseball diamond. It has four bases, home, first, second, and third base. First, let's look at this from the perspective of the batter, whom starts the at-bat from home base.

###Baseball Diamond


![](BaseballDiamond.png)

In our model, we want to model the possible states and transition of states that follow the pattern in which the batter runs across the bases. The batter must always start at home base, so that will be the initial state of the automaton.

Now, what is the next state? At first site, it seems any of the bases could be the next state, as a batter can run more than one base after hitting the ball. Depending on how far the ball is hit, a batter can score a single, double, or even a triple. However, even in the case of a double or triple, the batter *must* touch every base on his trip around the bases. Therefore, it would be incorrect to draw transitions directly from home base to second or third.

Additionally, the batter, once reaching home plate, scores a point, and cannot continue running around the bases. A special state exists, for when a batter walks off home base after scoring a run.

![](BaseballDiamond02.png)

The `run` label, symbolizes the input of running from one base to another. In baseball, there are more ways to get from one base to another, such as a batter being walked, but `run` will be treated as going from one base to another after the ball has been hit.

####Outs

As a batter runs around the bases, they may be tagged out at any time, if the basemen can manage to do so. A possible transition is needed to show what happens after a batter is tagged out. When one is out, be it through tagging or another rule, they must leave the diamond and return to the batters box. There is no way a player can return to a position on a base after being out. 

This means our baseball `FSA` has two final states, `Score` and `out`. A batter can be tagged out at every base, so every base has a possible transition to `out`. Lets look at our updated diagram.

![](BaseballDiamond03.png)

####Home-runs, Walks

In baseball, if a player hits the ball so far that it lands past the outfield wall, but does not go into the foul zones, the player is allowed to run across all the bases to home plate. This allows the batter to score a run without the possibility of being tagged out at any of the bases. Thus, we should add a special, direct state transition for the batter to the score final state, via the input of a home run.

A batter is permitted to safely transition to first base if the pitcher throws 4 *balls* in the at-bat. In this situation, the batter does not need to successfully hit the ball into live play, and is not truly running to first base, so we will add an additional input for that transition.

![](BaseballDiamond04.png)
