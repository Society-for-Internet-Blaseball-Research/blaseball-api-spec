# Blessing (bonus) Results

Get the results of one or more blessings/bonuses. Returns an array. Use commas to separate multiple blessing/bonus IDs.

## Endpoint

`https://www.blaseball.com/database/bonusResults?ids=:id1,:id2,...`

## Response

```json
[
    {
        "id": "7ce7eeb6-6abb-461c-b506-c10983e708a4",
        "bonusId": "max_random_player",
        "bonusTitle": "Bloodlust",
        "userId": "91aed555-1d2f-4baf-ad7f-501169fdb2e9",
        "teamId": "747b8e4a-7e50-4638-a973-ea7950a3e739",
        "totalVotes": 8312,
        "description": "Yazmin Mason's pitching stats were maxed out.",
        "teamVotes": 805,
        "highestTeam": "878c1bf6-0d21-4659-bfee-916c8314d69c",
        "highestTeamVotes": 1017
    },
    {
        "id": "df254f3d-3690-4417-bd6f-be2a231a7c25",
        "bonusId": "send_worst_hitter",
        "bonusTitle": "Exile",
        "userId": "1fce6956-c442-4c19-b88e-7de644fbdc31",
        "teamId": "747b8e4a-7e50-4638-a973-ea7950a3e739",
        "totalVotes": 4760,
        "description": "Hades Tigers sent the New York Millennials their worst hitter, Alyssa Harrell, and got back a random hitter, Mclaughlin Scorpler.",
        "teamVotes": 80,
        "highestTeam": "adc5b394-8f76-416d-9ce9-813706877b84",
        "highestTeamVotes": 1282
    },
    {
        "id": "f484ba2e-acbe-4b8f-bbe9-b361374afba7",
        "bonusId": "send_worst_pitcher",
        "bonusTitle": "Go Away",
        "userId": "fb1babbf-184d-408b-b505-ccf501d25175",
        "teamId": "23e4cbc1-e9cd-47fa-a35b-bfa06f726cb7",
        "totalVotes": 5947,
        "description": "Philly Pies sent the Charleston Shoe Thieves their worst pitcher, Kevin Dudley, and got back a random pitcher, Forrest Bookbaby.",
        "teamVotes": 1354,
        "highestTeam": "23e4cbc1-e9cd-47fa-a35b-bfa06f726cb7",
        "highestTeamVotes": 1354
    }
]
```

## Field Descriptions

**`id`**: The hexadecimal ID of the blessing/bonus.

**`bonusId`**: The name id of the blessing/bonus.

**`bonusTitle`**: The title displayed on the elections page.

**`userId`**: Unknown

**`teamId`**: Team that got the blessing/bonus

**`totalVotes`**: How many votes this blessing/bonus got.

**`description`**: The description for this blessing/bonus on the elections page.

**`teamVotes`**: The number of votes from the team who got this blessing/bonus. (Added Season 2)

**`highestTeam`**: The team that placed the most votes on this blessing/bonus. (Added Season 2)

**`highestTeamVotes`**: The amount of votes by the team that voted the most on this blessing/bonus. (Added Season 2)
