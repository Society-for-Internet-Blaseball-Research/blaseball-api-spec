# League Details

Returns inforation for a given league ID.

## Endpoint

`https://www.blaseball.com/database/league?id=:league_id`

## Response

```json
{
  "subleagues": [
    "7d3a3dd6-9ea1-4535-9d91-bde875c85e80",
    "93e58443-9617-44d4-8561-e254a1dbd450"
  ],
  "id":"d8545021-e9fc-48a3-af74-48685950a183",
  "name":"Internet League Blaseball",
  "tiebreakers":"72a618ed-c61c-4162-a455-3959a2d0e738"
}
```

## Field Descriptions

**`subleagues`**: The IDs of the subleagues that belong to the league.

**`id`**: The ID of the league.

**`name`**: The name of the league.

**`tiebreakers`**: The ID of a tiebreaker, unclear what this is.