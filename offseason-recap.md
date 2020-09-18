# Election Recap

Information about the decrees and bonuses that passed for a given season number (zero indexed).

## Endpoint

`https://www.blaseball.com/database/offseasonRecap?season=:season_number`

## Response

```json
{
  "id": "dfb49299-a2cc-40b4-b1c3-f4444beb7336",
  "bonusResults": [
    "cbb567c0-d770-4d22-92f6-ff16ebb94758",
    "0d3ea692-e151-4629-8f88-d75b56107ebc",
    "06a455d4-6bbc-4820-9256-e5c89e327720",
    "b40b4946-9f1c-4328-969f-20fae50dc47e",
    "ab2b02b4-935d-403e-81fc-d39c3e7c95ee",
    "8b5fb689-1d47-473a-bfa1-2d3ca26426ed",
    "468fcd69-fad7-4364-8426-24900db3e609",
    "268580d3-7bbd-474d-a563-08044bafda8b",
    "nagomi_mystery",
    "winniehess_mystery"
  ],
  "decreeResults": [
    "b090fdfc-7d9d-414b-a4a5-bbc698028c15"
  ],
  "name": "The Season 1 Election",
  "season": 0,
  "totalBonusVotes": 1295,
  "totalDecreeVotes": 925,
  "voteCount": 2220
}
```

## Field Descriptions

**`id`**: The ID for the offseason recap object.

**`bonusResults`**: List of the season's bonuses (in Season 1 only, two of the bonuses are not uuids but instead the bonus ID as from the Offseason Setup endpoint).

**`decreeResults`**: List of the decrees that passed.

**`name`**: The name of the Election.

**`season`**: The season number (zero indexed).

**`totalBonusVotes`**: The total number of votes for blessings/bonuses this season.

**`totalDecreeVotes`**: The total number of votes for decrees this season.

**`voteCount`**: The total number of votes this season.
