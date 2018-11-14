## Phase IV : Time Limits

The product is just about to be released and the final QA phase has found that the _Game Time_ value generated in the engine is unreliable in the extreme on the newest hardware.  It has been decided that the routine is to be scrapped and so the value can't be provided to generate the energy calculations made in [phase 2](phase2).

Instead the _GameContext_ object has a start time (in UTC) for the game that can be used as a starting point to calculate the current game running time.

The relevant portion of code is as below.  Please include this in your solution and use it to provide the relevant data.

```` csharp

    public sealed class GameContext {

        public GameContext() {
            GameStarted = DateTime.Now;
        }

        public DateTime GameStarted {get; private set;}

        public DateTime GameTime{
            get{
                return DateTime.Now;
            }
        }
    }

````