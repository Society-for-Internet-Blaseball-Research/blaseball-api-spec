# Game by ID Details

Returns the last broadcast game update for a given game ID. Completed games will show the final update of the game, currently running games will show the update present on www.blaseball.com, and future games will show a placeholder update if the game is already scheduled.

## Endpoint

`https://www.blaseball.com/database/gameById/:game_id`

## Response

Returns a single game update object. See the [game object](game-object.md) page for a centralized definition of what a game update contains.
