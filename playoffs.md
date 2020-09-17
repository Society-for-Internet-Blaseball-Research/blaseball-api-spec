# Playoffs

Get details about the playoffs for a given season number (zero indexed).

## Endpoint

`https://www.blaseball.com/database/playoffs?number=:season_number`

## Response

```json
{
  "id": "d30b9002-6e9d-4c31-bb86-68b69ad32a75",
  "name": "Season 4 Postseason",
  "numberOfRounds": 3,
  "playoffDay": 12,
  "rounds": [
    "b435ba04-dd90-4454-a123-6bd10989a6eb",
    "def46e3e-3cec-410c-985d-4decef431eb6",
    "a46cf811-3202-4d5d-98aa-c8965337702c"
  ],
  "season": 3,
  "tomorrowRound": 2,
  "winner": "747b8e4a-7e50-4638-a973-ea7950a3e739"
}
```

## Field Descriptions

**`id`**: The ID for the playoff object

**`name`**: The name of the playoffs.

**`numberOfRounds`**: Number of rounds in the playoffs.

**`playoffDay`**: Current day of the playoffs (zero indexed).

**`rounds`**: A list of round IDs that can be looked up using the [playoff round](playoff-round.md) endpoint.

**`season`**: The season number for the playoffs (zero indexed).

**`tomorrowRound`**: The index of tomorrow's round in rounds.

**`winner`**: The ID of the team that won the playoffs.
