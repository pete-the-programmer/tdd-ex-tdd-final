# TDD Final Exercise

In this exercise we start from a blank slate and build the solution __Test First__.  Please complete each phase before even looking at the next one.

## The beginning...

Welcome to _Total Complexity Games_, maker of games that maximise the fun by maximising the complexity of the scoring!

Word has come down from on high that we need _you_ to write the main code for calculating the score in our new game __Complicashooter__.  Not all the details have come out yet, but the main requirements are:

1. The _Game Experience_ department have decided that the players can choose between two kinds of __characters__ that make up the basis of the game.  The __Tortoises__ get more points per prize but are slow, and the __Hares__ that are fast but with less luck.  They have drawn up a table of the character's traits.

    | Character | Speed | Prize Worth | 
    |-----------|------:|------------:|
    | Tortoise  | 10.5  |        8    |
    | Hare      | 15.7  |        3    |

1. The _Business Analysis_ team have analysed these requirements and produced a simple truth table for desired outputs of the function given a set of inputs.

    | Character | time | numberPrizes | __Score__ |
    |-----------|-----:|-------------:|----------:|
    | Tortoise  |   1 |             1 |     18.5  |
    | Tortoise  |   10 |            1 |     113   |
    | Tortoise  |   10 |            3 |     129   |
    | Tortoise  |   15 |            3 |     181.5 |
    | Hare      |   1  |            1 |     18.7  |
    | Hare      |   10 |            1 |     160   |
    | Hare      |   15 |            3 |     244.5 |
