# Player Statsheet

Get the statsheets for one or more players. Returns an array. Use commas to separate multiple player statsheet IDs.

Keep in mind that each player statsheet is associated with a particular game, so the listed stats are only for that game.

## Endpoint

`https://www.blaseball.com/database/playerSeasonStats?ids=:id1,:id2,...`

## Response

```json
[
  {
    "id": "ae2e7d89-4b96-464f-9556-1f669a95be1a",
    "playerId": "7b55d484-6ea9-4670-8145-986cb9e32412",
    "teamId": "979aee4a-6d80-4863-bf1c-ee1a78e06024",
    "team": "Hawaii Fridays",
    "name": "Stevenson Heat",
    "atBats": 0,
    "caughtStealing": 0,
    "doubles": 0,
    "earnedRuns": 1,
    "groundIntoDp": 0,
    "hits": 0,
    "hitsAllowed": 8,
    "homeRuns": 0,
    "losses": 0,
    "outsRecorded": 27,
    "rbis": 0,
    "runs": 0,
    "stolenBases": 0,
    "strikeouts": 7,
    "struckouts": 0,
    "triples": 0,
    "walks": 0,
    "walksIssued": 0,
    "wins": 1
  }
]
```

## Field Descriptions

**`id`**: The id for the player statsheet.

**`playerId`**: The ID of the player.

**`teamId`**: An array containing the number of runs per inning.

**`team`**: The name of the team the player is on.

**`name`**: The name of the player.

**`atBats`**: The number of atBats the player had in this game.

**`caughtStealing`**: The number of times the player was caught stealing this game.

**`doubles`**: The number of doubles the player has hit this game.

**`earnedRuns`**: The number of earned runs for this player for this game.

**`groundIntoDp`**: The number of groundouts into double plays for this player this game.

**`hits`**: The number of hits this player has had this game.

**`homeruns`**: The number of home runs this player has had this game.

**`losses`**: For one player each game this field is set to 1 if their team lost.

**`outsRecorded`**: The number of outs this player has recorded this game.

**`rbis`**: The number of RBIs this player has had this game.

**`runs`**: The number of runs this player has had this game.

**`stolenBases`**: The number of bases this player has stolen this game.

**`strikeouts`**: The number of strikeouts this player has had this game.

**`triples`**: The number of triples this player has had this game.

**`walks`**: The number of walks this player has had this game.

**`walksIssued`**: The number of walks this player has issued this game.

**`wins`**: For one player each game this field is set to 1 if their team won.
