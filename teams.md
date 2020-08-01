# Team Details

Returns limited stats, player IDs, and other information for a given team ID. Limited to a single team ID.

## Endpoint

`https://blaseball.com/database/team?id=:id`

## Response

```json
[
  {
    "lineup": [
      "1ba715f2-caa3-44c0-9118-b045ea702a34",
      "26cfccf2-850e-43eb-b085-ff73ad0749b8",
      "13a05157-6172-4431-947b-a058217b4aa5",
      "80dff591-2393-448a-8d88-122bd424fa4c",
      "667cb445-c288-4e62-b603-27291c1e475d",
      "15ae64cd-f698-4b00-9d61-c9fffd037ae2",
      "083d09d4-7ed3-4100-b021-8fbe30dd43e8",
      "06ced607-7f96-41e7-a8cd-b501d11d1a7e",
      "66cebbbf-9933-4329-924a-72bd3718f321"
    ],
    "rotation": [
      "1732e623-ffc2-40f0-87ba-fdcf97131f1f",
      "9786b2c9-1205-4718-b0f7-fc000ce91106",
      "b082ca6e-eb11-4eab-8d6a-30f8be522ec4",
      "60026a9d-fc9a-4f5a-94fd-2225398fa3da",
      "814bae61-071a-449b-981e-e7afc839d6d6"
    ],
    "bullpen": [
      "0672a4be-7e00-402c-b8d6-0b813f58ba96",
      "62111c49-1521-4ca7-8678-cd45dacf0858",
      "7f379b72-f4f0-4d8f-b88b-63211cf50ba6",
      "906a5728-5454-44a0-adfe-fd8be15b8d9b",
      "90cc0211-cd04-4cac-bdac-646c792773fc",
      "a7b0bef3-ee3c-42d4-9e6d-683cd9f5ed84",
      "b85161da-7f4c-42a8-b7f6-19789cf6861d",
      "d2a1e734-60d9-4989-b7d9-6eacda70486b"
    ],
    "bench": [
      "20395b48-279d-44ff-b5bf-7cf2624a2d30",
      "d8bc482e-9309-4230-abcb-2c5a6412446d",
      "cd5494b4-05d0-4b2e-8578-357f0923ff4c"
    ],
    "seasonAttributes":[],
    "permanentAttributes":[],
    "_id":"23e4cbc1-e9cd-47fa-a35b-bfa06f726cb7",
    "fullName":"Philly Pies",
    "location":"Philly",
    "mainColor":"#399d8f",
    "nickname":"Pies",
    "secondaryColor":"#ffffff",
    "shorthand":"PHIL",
    "emoji":"0x1F967",
    "slogan":"Pie or Die.",
    "shameRuns":0,
    "totalShames":4,
    "totalShamings":0,
    "seasonShames":4,
    "seasonShamings":8,
    "championships":1
  }
]
```

## Field Descriptions

**`lineup`**: The IDs of the players that belong to the team's lineup.

**`rotation`**: The IDs of the players that belong to the team's pitching rotation.

**`bullpen`**: The IDs of the players that belong to the team's bullpen.

**`bench`**: The IDs of the players that belong to the team's bench.

**`seasonAttributes`**: The IDs of attributes assigned to the team for this season.

**`permanentAttributes`**: The IDs of attributes assigned to the team permanently.

**`fullName`**: The full name of the team.

**`location`**: The home city of the team.

**`mainColor`**: The hex code of the team's primary color.

**`nickname`**: The team's nickname.

**`secondaryColor`**: The hex code of the team's secondary color.

**`shorthand`**: The abbreviated team name.

**`emoji`**: The team's emoji.

**`slogan`**: The team's slogan.

**`shameRuns`**: ?

**`totalShames`**: ?

**`totalShamings`**: ?

**`seasonShames`**: ?

**`seasonShamings`**: ?

**`championships`**: ?