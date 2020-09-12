# Game Statsheet

Get the statsheets for one or more games. Returns an array. Use commas to separate multiple game statsheet IDs.

## Endpoint

`https://www.blaseball.com/database/gameStatsheets?ids=:id1,:id2,...`

## Response

```json
{
  "id": "cfe83059-4340-4809-adf8-bf84bce096a7",
  "homeTeamRunsByInning": [1, 1, 1, 0, 2, 2, 0, 0],
  "awayTeamRunsByInning": [0, 0, 0, 0, 0, 0, 0, 0, 1],
  "awayTeamTotalBatters": 0,
  "homeTeamTotalBatters": 0,
  "awayTeamStats": "72f85011-327b-4510-a85b-c0f3009eebfe",
  "homeTeamStats": "d8a5fc41-9ab3-4355-8bb0-dae297aaf958"
}
```

## Field Descriptions

**`id`**: The id for the game statsheet.

**`homeTeamRunsByInning`**: An array containing the number of runs per inning.

**`homeTeamRunsByInning`**: An array containing the number of runs per inning.

**`awayTeamTotalBatters`**: Seems broken (always 0).

**`homeTeamTotalBatters`**: Seems broken (always 0).

**`awayTeamStats`**: The ID of the away team statsheet.

**`homeTeamStats`**: The ID of the home team statsheet.
