# Simplified state machine of a 4 years old child.

_**Very Important:**_ _Please, do not fork this repository so we can avoid exposing the possible solutions on the web!_


## Goal:
Build a state machine based on the diagram below in your favourite language.
The initial state is playing.

![States](states.png?raw=true "States")

## Constraints:
* You cannot use any third party library.
* Every transition should be printed on screen containing the "from" and "to" state in a readable sentence.
* Impossible transitions should not change state but print a msg similar to: "Cannot transition from [current state] with [call]"

## Bonus
Child has two new properties:
* mood - int (initial: 0)
* snacks - int (initial: 0)

Snacks can be given to the child only when he is in the playing or eating state.

Snacks are consumed before the child transitions from the eating state to the playing state.

Snacks raise the mood when consumed:
* every third snack raises it by 2
* every fifth snack raises it by 4
* every fifteenth snack raises it by 8
* every other snack raises it by 1

mood falls back to 0 when state transitions to hiding
