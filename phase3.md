## Phase II : Energy

So far so good.

Ms. Lovejoy in charge of _Customer Turnover_ always says 

> a short game is a good game

...especially when the players pay for every game started.

Now each player is allotted 100 __energy blocks__, which run down at a rate of 1 per second.  When the energy hits zero the game is over.

However, the _Player Gamification_ team thinks that it would be fun to allow players the option to __trade-in points__ for another 50 energy blocks when the energy gets down below 5, at a rate of 8 points for _Tortoises_ and 7 points for _hares_.

Bob in the main _Game Engine Developers_ pod says that it's too difficult to store the number of times a player trades in for more time, but cheerfully says that he has a _GameContext_ object that can provide the _Game Duration_ and let you "sort it out from there".

So, the score can now be calculated as:

| Character | Number Prizes | Game Duration (s) | __Score__ | __Energy__ |
|-----------|--------------:|------------------:|----------:|-----------:|
| Tortoise  |             0 |               0   |     -15.7 |        100 |
| Tortoise  |             7 |              20   |      40.3 |         80 |
| Tortoise  |             7 |              99   |      40.3 |          1 |
| Tortoise  |             7 |             101   |      32.3 |         49 |
| Tortoise  |             7 |             151   |      24.3 |         49 |
| Hare      |             7 |              20   |      15.5 |         80 |
| Hare      |             7 |             101   |       8.5 |         49 |
| Hare      |             7 |             153   |       1.5 |         47 |


### Next step

Don't move on until you have completely finished this page.

When you have finished, you may move on to [phase 4](phase4)