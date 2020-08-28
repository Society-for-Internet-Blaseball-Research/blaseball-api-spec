# Playoffs

Get details about the playoffs for a season.

## Endpoint

`https://blaseball.com/database/playoffs?number=:season`

## Response

```json
{
    "rounds": [
        "aecb79df-5f61-40c1-a244-8a42268f2e4c",
        "2ba38446-ec15-405f-b5e6-c9eb2ab266bc",
        "b8f24ce6-bd6b-45f5-89a8-d5372444e9e4"
    ],
    "id": "0e8512d6-648d-40bf-bbbd-c4e7690c9ce1",
    "__v": 0,
    "name": "Season 3 Postseason",
    "numberOfRounds": 3,
    "playoffDay": 13,
    "season": 2,
    "tomorrowRound": 2,
    "winner": "747b8e4a-7e50-4638-a973-ea7950a3e739"
}
```

## Field Descriptions

**`rounds`**: List of playoff rounds.

**`name`**: Name of the playoffs.

**`numberOfRounds`**: Number of rounds in the playoffs.

**`playoffDay`**: Current day of the playoffs.

**`season`**: Season number.

**`tomorrowRound`**: Index in rounds.

**`winner`**: Team that won the playoffs.