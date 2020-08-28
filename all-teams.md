# All Teams

Returns a list of team definitions for every team in the league.

## Endpoint

`https://blaseball.com/database/allTeams`

## Response

```json
[
  {
    "lineup": [
      "2f3d7bc7-6ffb-40c3-a94f-5e626be413c9",
      "4941976e-31fc-49b5-801a-18abe072178b",
      "57448b62-f952-40e2-820c-48d8afe0f64d",
      "b3d518b9-dc68-4902-b68c-0022ceb25aa0",
      "8a6fc67d-a7fe-443b-a084-744294cec647",
      "3a96d76a-c508-45a0-94a0-8f64cd6beeb4",
      "1e8b09bd-fbdd-444e-bd7e-10326bd57156",
      "c0732e36-3731-4f1a-abdc-daa9563b6506",
      "9ac2e7c5-5a34-4738-98d8-9f917bc6d119"
    ],
    "rotation": [
      "7b55d484-6ea9-4670-8145-986cb9e32412",
      "bd549bfe-b395-4dc0-8546-5c04c08e24a5",
      "167751d5-210c-4a6e-9568-e92d61bab185",
      "7158d158-e7bf-4e9b-9259-62e5b25e3de8",
      "89ec77d8-c186-4027-bd45-f407b4800c2c"
    ],
    "bullpen": [
      "a2483925-697f-468f-931c-bcd0071394e5",
      "527c1f6e-a7e4-4447-a824-703b662bae4e",
      "62823073-84b8-46c2-8451-28fd10dff250",
      "805ba480-df4d-4f56-a4cf-0b99959111b5",
      "cd6b102e-1881-4079-9a37-455038bbf10e",
      "3954bdfa-931f-4787-b9ac-f44b72fe09d7",
      "ccc99f2f-2feb-4f32-a9b9-c289f619d84c",
      "fbb5291c-2438-400e-ab32-30ce1259c600"
    ],
    "bench": [
      "03d06163-6f06-4817-abe5-0d14c3154236",
      "960f041a-f795-4001-bd88-5ddcf58ee520",
      "0bd5a3ec-e14c-45bf-8283-7bc191ae53e4"
    ],
    "seasonAttributes": [],
    "permanentAttributes": [],
    "id": "979aee4a-6d80-4863-bf1c-ee1a78e06024",
    "fullName": "Hawaii Fridays",
    "location": "Hawaii",
    "mainColor": "#3ee652",
    "nickname": "Fridays",
    "secondaryColor": "#e67575",
    "shorthand": "HF",
    "emoji": "0x1F3DD",
    "slogan": "It's Island Time!",
    "shameRuns": 0,
    "totalShames": 4,
    "totalShamings": 0,
    "seasonShames": 4,
    "seasonShamings": 8,
    "championships": 0
  }
]
```

## Field Descriptions

**`lineup`**: IDs of the players on the team's fielded roster.

**`rotation`**: IDs of the team's starting pitchers.

**`bullpen`**: IDs of the players in the team's bullpen.

**`bench`**: IDs of the players on the team's roster, but are not available in a game.

**`seasonAttributes`**: The IDs of attributes assigned to the team for this season.

**`permanentAttributes`**: The IDs of attributes assigned to the team permanently.

**`fullName`**: The full name (location + nickname) of the team.

**`location`**: The location in which the team is based.

**`mainColor`**: The background color of the team's icon.

**`nickname`**: The team's unique noun descriptor.

**`secondaryColor`**: The foreground color of the team's icon.

**`shorthand`**: The scorecard abbreviation for the team.

**`emoji`**: The emoji that represents the team.

**`slogan`**: The team's slogan.

**`shameRuns`**: The number of runs the team has given up while shamed. To be possibly used if Enhanced Shame is decreed.

**`totalShames`**: The number of times the team has been shamed across all seasons.

**`totalShamings`**: The number of times the team has shamed another team across all seasons.

**`seasonShames`**: The number of times the team has been shamed this season.

**`seasonShamings`**: The number of times the team has shamed another team across this season.

**`championships`**: The number of seasons the team has won.
