# ucinewgame

`GUI -> Engine`

Sent to the engine when the next search (started with [[position]] and [[go]]) will be from a different game.

The GUI should always send [[isready]] after [ucinewgame] to wait for the engine to finish its operation.

#Tags
[GUI to Engine]