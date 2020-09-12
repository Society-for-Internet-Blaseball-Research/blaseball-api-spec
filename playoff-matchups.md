# Playoff Matchups

Get information about one or more playoff matchups. Returns an array. Use commas to separate multiple playoff matchup IDs.

## Endpoint

`https://www.blaseball.com/database/playoffMatchups?ids=:id1,:id2,...`

## Response

```json
[
  {
    "id": "1a531d31-5ec2-45a1-9ea0-004236139d59",
    "name": null,
    "awaySeed": 1,
    "awayTeam": "36569151-a2fb-43c1-9df7-2df512424c82",
    "awayWins": 3,
    "homeSeed": 0,
    "homeTeam": "ca3f1c8c-c025-4d8e-8eef-5be6accbeb16",
    "homeWins": 2
  }
]
```

## Field Descriptions

**`id`**: The ID of the playoff matchup.

**`name`**: Matchup name. (null?)

**`awaySeed`**: The seed for the away team in this matchup.

**`awayTeam`**: The ID of the away team for this matchup.

**`awayWins`**: The current number of wins for the away team in this matchup.

**`homeSeed`**: The seed for the home team in this matchup.

**`homeTeam`**: The ID of the home team for this matchup.

**`homeWins`**: The current number of wins for the home team in this matchup.
