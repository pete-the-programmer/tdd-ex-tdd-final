---
title: TDD Final Exercise
description: Pete the Programmer
---

# TDD Final Exercise

In this exercise we start from a blank slate and build the solution __Test First__.  Please complete each phase before even looking at the next one.

## The beginning...

Welcome to _Total Complexity Games_, maker of games that maximise the fun by maximising the complexity of the scoring!

Word has come down from on high that we need _you_ to write the main code for calculating the score in our new game __Complica__.  Not all the details have come out yet, but the main requirements are:

1. The _Game Research_ department have decided that the players can choose between two kinds of __characters__ that make up the basis of the game.  The __Tortoises__ get more points per prize but cost more to start with, and the __Hares__ that are cheap and can move more quickly, but they have lower prize values.  They have drawn up a table of the character's traits.

    | Character | Initial Cost | Prize Worth | 
    |-----------|-------------:|------------:|
    | Tortoise  |        15.7  |        8    |
    | Hare      |         5.5  |        3    |

1. The _Business Analysis_ team have analysed these requirements and produced a simple truth table for desired outputs of the function given a set of inputs.

    | Character | numberPrizes | __Score__ |
    |-----------|-------------:|----------:|
    | Tortoise  |            1 |     -7.7  |
    | Tortoise  |            2 |      0.3  |
    | Tortoise  |            3 |      8.3  |
    | Hare      |            1 |     -2.5  |
    | Hare      |            5 |      9.5  |

## Instructions

Writing the tests first, create a calculator that can generate the score for a selected character and number of prizes opened.

HINT: Write a test case for each row of the BA's table.  Make each row go green _before_ moving to the next row.

## Next step

Don't move on until you have completely finished this page.

When you have finished, you may move on to [phase 2](phase2.md)
