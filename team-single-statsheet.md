# Single Team Statsheet

## Deprecated

**DO NOT USE THIS ENDPOINT**. Use the [team statsheet](team-statsheet.md) endpoint instead. This endpoint can only fetch the statsheet for a single team and using it repeatedly would cause unnecessary load on the Blaseball servers.

Get the statsheet for a given team. Keep in mind that a team statsheet is associated with a given game so the player stats are only for that game and the list of players are only those who played in that game. If you need to get more than one statsheet

## Endpoint

`https://www.blaseball.com/database/teamStatsheet?id=:statsheetId`

## Response

```json
{
  "id": "9298cca4-442e-4aa0-8bcf-8ee349b1a45e",
  "playerStats": [
    "323cec58-c2ee-4ca0-a8a0-f51b8ce2be6a",
    "03fb7c2a-cb80-4506-b898-8082d5f56e29",
    "53db624f-cb86-4e44-b6cf-54fa5d5ab113",
    "67761681-03aa-4ca9-afc0-387bef14f8fe",
    "962edbdc-e77c-43b8-93ee-ecd97a5bfe16",
    "5f484372-53b9-4057-aac2-e8411130e7b8",
    "ac20046b-2868-4eff-ad9b-977c78b5a121",
    "d12fc287-b0ff-472a-abf4-5c9615742263",
    "bbfbc547-fc5f-4b75-8288-68c81d2299fa",
    "0a70f69e-5767-4be7-946e-d0969ad15851"
  ],
  "gamesPlayed": 0,
  "wins": 0,
  "losses": 0,
  "name": "Yellowstone Magic",
  "teamId": "7966eb04-efcc-499b-8f03-d13916330531"
}
```

## Field Descriptions

**`id`**: The id for the team statsheet.

**`playerStats`**: An array of IDs for each players's statsheet.

**`gamesPlayed`**: Seems broken (always 0).

**`wins`**: Seems broken (always 0).

**`losses`**: Seems broken (always 0).

**`name`**: The Name of the team.

**`teamId`**: The ID of the team.
