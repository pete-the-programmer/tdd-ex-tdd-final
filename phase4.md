## Phase IV : Time of Day Bonus

The product is just about to be released and the _Product Launch Tiger Team_ has reminded everyone that 
in the supplementary documentation kept in the business section of the CRM it states:
> every player that starts a game between the __11th of June 2018 at 9am__ and the __17 of July 2018 at 5pm__ (UTC) will get a bonus of _30 points_ at the start of the game.

Bob says that you can access the _GameContext_ object directly to get the current date/time as well as the game's duration.  You will be expected to refactor your code to use this object instead of the duration value in the previous phase.

_NOTE_: Please include the following reference code in your solution to provide the game context.

```` csharp
    public interface IGameContext {
        DateTime StartedTime {get;}
        DateTime CurrentTime {get;}
        int GameDuration {get;}
    }

    public class GameContext: IGameContext {

        public GameContext() {
            StartedTime = DateTime.UtcNow;
        }

        public DateTime StartedTime {get; private set;}

        public DateTime CurrentTime {
            get {
                return DateTime.UtcNow;
            }
        }

        public int GameDuration {
            get {
                return (int)(CurrentTime - StartedTime).TotalSeconds;
            }
        }
    }

````

__Your mission__ is to add these bonus rules to the scoring calculator, remembering to check the boundaries either side of the bonus time window.

---

### Fin