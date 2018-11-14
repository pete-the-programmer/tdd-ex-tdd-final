## Phase II : Energy

So far so good.

Ms. Lovejoy in charge of _Customer Turnover_ always says 

> a short game is a good game

...especially when the players pay for every game started.

Now each player is allotted 100 __energy blocks__, which run down at a rate of 1 per second.  When the energy hits zero the game is over.

However, the _Player Gamification_ team thinks that it would be fun to allow players to __trade-in points__ for another 50 energy blocks, at a rate of 10 points for _Tortoises_ and 12 points for _hares_. 

Bob in the main _Game Engine Developers_ pod says that it's too difficult to store the number of times a player trades in for more time, but cheerfully says that there is a _GameContext_ object that includes the game start time and let you "sort it out from there".

So, the score can now be calculated as:

| Character | Number Prizes | Game Time (s) | __Score__ | __Energy__ |
|-----------|--------------:|--------------:|----------:|-----------:|
| Tortoise  |             0 |           0   |       0.0 |        100 |
| Tortoise  |            10 |          20   |      64.3 |         80 |
| Tortoise  |            10 |          99   |      64.3 |          1 |
| Tortoise  |            10 |         101   |      54.3 |         99 |
| Tortoise  |            10 |         151   |      44.3 |         99 |
| Hare      |            10 |          20   |      24.5 |         80 |
| Hare      |            10 |         101   |      12.5 |         99 |
| Hare      |            10 |         153   |       0.5 |         97 |


NOTE: Please include the following reference code in your solution to provide the game context.

```` csharp

    public sealed class GameContext {

        public GameContext() {
            GameStarted = DateTime.UtcNow;
        }

        public DateTime StartedTime {get; private set;}

        public DateTime CurrentTime{
            get{
                return DateTime.Now;
            }
        }
    }

````

### Next step

Don't move on until you have completely finished this page.

When you have finished, you may move on to [phase 3](phase3)