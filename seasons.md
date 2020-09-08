# Season Details

Returns inforation for a given season number (zero indexed).

## Endpoint

`https://www.blaseball.com/database/season?number=:season_number`

## Response

```json
{
  "id": "9465ef83-c4c7-4aaa-83d0-d78854652618",
  "league": "d8545021-e9fc-48a3-af74-48685950a183",
  "rules": "4ae9d46a-5408-460a-84fb-cbd8d03fff6c",
  "schedule": "de797ddc-e17f-4530-a336-ff13411a5c88",
  "seasonNumber": 4,
  "standings": "48789741-69b1-4aa9-a46c-eda3351a3f5e",
  "stats": "51c29a58-a4c6-435a-8c60-ab49a493d98f",
  "terminology": "b67e9bbb-1495-4e1b-b517-f1444b0a6c8b"
}
```

## Field Descriptions

**`id`**: The ID of the season.

**`league`**: The ID of the league that is playing in the season.

**`rules`**: The ID of the rules for the season. Unknown what this ID goes to.

**`schedule`**: The ID of the schedule for the season. Unknown what this ID goes to.

**`seasonNumber`**: The season number (zero indexed)

**`standings`**: The ID of the standings for the season. Goes to the [standings](standings.md) endpoint.

**`stats`**: The ID of the statsheet for the season. Goes to the [season statsheet](season-statsheet.md) endpoint.

**`terminology`**: The ID of the terminology for the season. Unknown what this ID goes to.