# Data Stream Details

This is the endpoint that the site uses to stream live game data to the www.blaseball.com site. It uses [Server Sent Events](https://en.wikipedia.org/wiki/Server-sent_events). Every few seconds it sends a single "data" event. The event is rather large so below it has been broken down into "Overview" and "Full Response" sections.

## Endpoint

`https://www.blaseball.com/events/streamData`

## Overview

```javascript
data: {
  "value": {
    "games": {
      "sim": { /* SIM_OBJECT */ },
      "season": { /* SEASON OBJECT */ },
      "standings": { /* STANDINGS OBJECT */ },
      "schedule": { /* ARRAY WITH 10 GAME OBJECTS */ },
      "tomorrowSchedule": { /* ARRAY WITH 10 GAME OBJECTS */ },
      "postseason": { /* POSTSEASON OBJECT */ }
    },
    "leagues": {
      "teams": { /* ARRAY WITH 20 TEAM OBJECTS */ },
      "subleagues": { /* ARRAY WITH 2 SUBLEAGUE OBJECTS */ },
      "divisions": { /* ARRAY WITH 4 DIVISION OBJECTS */ },
      "leagues": { /* ARRAY WITH 1 LEAGUE OBJECT */ }
    },
    "temporal": { /* TEMPORAL OBJECT */ }
  }
}
```


## Full Response

```javascript
data: {
  "value": {
    "games": {
      "sim": {
        "id": "thisidisstaticyo",
        "day": 75,
        "league": "d8545021-e9fc-48a3-af74-48685950a183",
        "nextElectionEnd": "2020-09-06T19:00:00.411Z",
        "nextPhaseTime": "2020-08-31T16:00:00.354Z",
        "nextSeasonStart": "2020-09-07T16:00:00.412Z",
        "phase": 2,
        "playOffRound": 0,
        "playoffs": "d30b9002-6e9d-4c31-bb86-68b69ad32a75",
        "rules": "4ae9d46a-5408-460a-84fb-cbd8d03fff6c",
        "season": 4,
        "seasonId": "9465ef83-c4c7-4aaa-83d0-d78854652618",
        "terminology": "b67e9bbb-1495-4e1b-b517-f1444b0a6c8b",
        "eraColor": "#ff0000",
        "eraTitle": "The Discipline Era",
        "twgo": "JHFMTOJMNPSMLMDGFOSEZDTMJWHPADAACGRTBBPBBCJRTPMJCSNKKAOMVMSTAJTVTCJIMPSSSTBFHRSSMSDKIRLWLVWSSMEIMCCDMDRT",
        "subEraColor": "#61b3ff",
        "subEraTitle": "Reverb",
        "attr": [
          "OPENED_BOOK",
          "UNLOCKED_PEANUTS",
          "EAT_THE_RICH",
          "UNLOCKED_INTERVIEWS"
        ]
      },
      "season": {
        "id": "9465ef83-c4c7-4aaa-83d0-d78854652618",
        "league": "d8545021-e9fc-48a3-af74-48685950a183",
        "rules": "4ae9d46a-5408-460a-84fb-cbd8d03fff6c",
        "schedule": "de797ddc-e17f-4530-a336-ff13411a5c88",
        "seasonNumber": 4,
        "standings": "48789741-69b1-4aa9-a46c-eda3351a3f5e",
        "stats": "51c29a58-a4c6-435a-8c60-ab49a493d98f",
        "terminology": "b67e9bbb-1495-4e1b-b517-f1444b0a6c8b"
      },
      "standings": {
        "id": "48789741-69b1-4aa9-a46c-eda3351a3f5e",
        "losses": {
          "b72f3061-f573-40d7-832a-5ad475bd7909": 26,
          "878c1bf6-0d21-4659-bfee-916c8314d69c": 58,
          "b024e975-1c4a-4575-8936-a3754a08806a": 38,
          "adc5b394-8f76-416d-9ce9-813706877b84": 37,
          "ca3f1c8c-c025-4d8e-8eef-5be6accbeb16": 32,
          "bfd38797-8404-4b38-8b82-341da28b1f83": 40,
          "3f8bbb15-61c0-4e3f-8e4a-907a5fb1565e": 43,
          "979aee4a-6d80-4863-bf1c-ee1a78e06024": 39,
          "7966eb04-efcc-499b-8f03-d13916330531": 41,
          "36569151-a2fb-43c1-9df7-2df512424c82": 31,
          "8d87c468-699a-47a8-b40d-cfb73a5660ad": 26,
          "23e4cbc1-e9cd-47fa-a35b-bfa06f726cb7": 41,
          "f02aeae2-5e6a-4098-9842-02d2273f25c7": 48,
          "57ec08cc-0411-4643-b304-0e80dbc15ac7": 40,
          "747b8e4a-7e50-4638-a973-ea7950a3e739": 31,
          "eb67ae5e-c4bf-46ca-bbbc-425cd34182ff": 32,
          "9debc64f-74b7-4ae1-a4d6-fce0144b6ea5": 44,
          "b63be8c2-576a-4d6e-8daf-814f8bcea96f": 45,
          "105bc3ff-1320-4e37-8ef0-8d595cb95dd0": 40,
          "a37f9158-7f82-46bc-908c-c9e2dda7c33b": 28
        },
        "wins": {
          "b72f3061-f573-40d7-832a-5ad475bd7909": 50,
          "878c1bf6-0d21-4659-bfee-916c8314d69c": 18,
          "b024e975-1c4a-4575-8936-a3754a08806a": 38,
          "adc5b394-8f76-416d-9ce9-813706877b84": 39,
          "ca3f1c8c-c025-4d8e-8eef-5be6accbeb16": 44,
          "bfd38797-8404-4b38-8b82-341da28b1f83": 36,
          "3f8bbb15-61c0-4e3f-8e4a-907a5fb1565e": 33,
          "979aee4a-6d80-4863-bf1c-ee1a78e06024": 37,
          "7966eb04-efcc-499b-8f03-d13916330531": 35,
          "36569151-a2fb-43c1-9df7-2df512424c82": 45,
          "8d87c468-699a-47a8-b40d-cfb73a5660ad": 50,
          "23e4cbc1-e9cd-47fa-a35b-bfa06f726cb7": 35,
          "f02aeae2-5e6a-4098-9842-02d2273f25c7": 28,
          "57ec08cc-0411-4643-b304-0e80dbc15ac7": 36,
          "747b8e4a-7e50-4638-a973-ea7950a3e739": 45,
          "eb67ae5e-c4bf-46ca-bbbc-425cd34182ff": 44,
          "9debc64f-74b7-4ae1-a4d6-fce0144b6ea5": 32,
          "b63be8c2-576a-4d6e-8daf-814f8bcea96f": 31,
          "105bc3ff-1320-4e37-8ef0-8d595cb95dd0": 36,
          "a37f9158-7f82-46bc-908c-c9e2dda7c33b": 48
        }
      },
      "schedule": [
        {
          "id": "87262a0b-63f0-4e36-9502-13ab1e2de55f",
          "basesOccupied": [],
          "baseRunners": [],
          "baseRunnerNames": [],
          "outcomes": [],
          "terminology": "b67e9bbb-1495-4e1b-b517-f1444b0a6c8b",
          "lastUpdate": "Game over.",
          "rules": "4ae9d46a-5408-460a-84fb-cbd8d03fff6c",
          "statsheet": "e5962e4e-d1f3-4af2-9434-2ce22c532d0c",
          "awayPitcher": "e6114fd4-a11d-4f6c-b823-65691bb2d288",
          "awayPitcherName": "Bevan Underbuck",
          "awayBatter": null,
          "awayBatterName": "",
          "awayTeam": "979aee4a-6d80-4863-bf1c-ee1a78e06024",
          "awayTeamName": "Hawaii Fridays",
          "awayTeamNickname": "Fridays",
          "awayTeamColor": "#3ee652",
          "awayTeamEmoji": "0x1F3DD",
          "awayOdds": 0.48003624252189786,
          "awayStrikes": 3,
          "awayScore": 0,
          "awayTeamBatterCount": 28,
          "homePitcher": "9397ed91-608e-4b13-98ea-e94c795f651e",
          "homePitcherName": "Yeong-Ho Garcia",
          "homeBatter": null,
          "homeBatterName": "",
          "homeTeam": "7966eb04-efcc-499b-8f03-d13916330531",
          "homeTeamName": "Yellowstone Magic",
          "homeTeamNickname": "Magic",
          "homeTeamColor": "#bf0043",
          "homeTeamEmoji": "0x2728",
          "homeOdds": 0.5199637574781021,
          "homeStrikes": 3,
          "homeScore": 6,
          "homeTeamBatterCount": 35,
          "season": 4,
          "isPostseason": false,
          "day": 75,
          "phase": 6,
          "gameComplete": true,
          "finalized": true,
          "gameStart": true,
          "halfInningOuts": 0,
          "halfInningScore": 0,
          "inning": 8,
          "topOfInning": true,
          "atBatBalls": 0,
          "atBatStrikes": 0,
          "seriesIndex": 1,
          "seriesLength": 3,
          "shame": false,
          "weather": 7,
          "baserunnerCount": 0
        },
        // ... 9 other game objects ...
      ],
      "tomorrowSchedule": [
        {
          "id": "0bf5b64b-0055-4af8-8b0e-c03bbb068fab",
          "basesOccupied": [],
          "baseRunners": [],
          "baseRunnerNames": [],
          "outcomes": [],
          "terminology": "b67e9bbb-1495-4e1b-b517-f1444b0a6c8b",
          "lastUpdate": "",
          "rules": "4ae9d46a-5408-460a-84fb-cbd8d03fff6c",
          "statsheet": "7838e886-5a02-4811-bd20-3143a216510f",
          "awayPitcher": "34267632-8c32-4a8b-b5e6-ce1568bb0639",
          "awayPitcherName": "Gunther O'Brian",
          "awayBatter": null,
          "awayBatterName": "",
          "awayTeam": "bfd38797-8404-4b38-8b82-341da28b1f83",
          "awayTeamName": "Charleston Shoe Thieves",
          "awayTeamNickname": "Shoe Thieves",
          "awayTeamColor": "#ffce0a",
          "awayTeamEmoji": "0x1F45F",
          "awayOdds": 0.2831501948584466,
          "awayStrikes": 3,
          "awayScore": 0,
          "awayTeamBatterCount": 0,
          "homePitcher": "81d7d022-19d6-427d-aafc-031fcb79b29e",
          "homePitcherName": "Patty Fox",
          "homeBatter": null,
          "homeBatterName": "",
          "homeTeam": "36569151-a2fb-43c1-9df7-2df512424c82",
          "homeTeamName": "New York Millennials",
          "homeTeamNickname": "Millennials",
          "homeTeamColor": "#ffd4d8",
          "homeTeamEmoji": "0x1F4F1",
          "homeOdds": 0.7168498051415535,
          "homeStrikes": 3,
          "homeScore": 0,
          "homeTeamBatterCount": 0,
          "season": 4,
          "isPostseason": false,
          "day": 76,
          "phase": 0,
          "gameComplete": false,
          "finalized": false,
          "gameStart": false,
          "halfInningOuts": 0,
          "halfInningScore": 0,
          "inning": 0,
          "topOfInning": true,
          "atBatBalls": 0,
          "atBatStrikes": 0,
          "seriesIndex": 2,
          "seriesLength": 3,
          "shame": false,
          "weather": 12,
          "baserunnerCount": 0
        },
        // ... 9 other game objects ...
      ],
      "postseason": {}
    },
    "leagues": {
      "teams": [
        {
          "id": "b72f3061-f573-40d7-832a-5ad475bd7909",
          "lineup": [
            "58c9e294-bd49-457c-883f-fb3162fc668e",
            "23110c0f-2cf9-4d9c-ab2d-634f2f18867e",
            "2b157c5c-9a6a-45a6-858f-bf4cf4cbc0bd",
            "11de4da3-8208-43ff-a1ff-0b3480a0fbf1",
            "126fb128-7c53-45b5-ac2b-5dbf9943d71b",
            "cbd19e6f-3d08-4734-b23f-585330028665",
            "ee55248b-318a-4bfb-8894-1cc70e4e0720",
            "0eea4a48-c84b-4538-97e7-3303671934d2",
            "bd24e18b-800d-4f15-878d-e334fb4803c4"
          ],
          "rotation": [
            "3c331c87-1634-46c4-87ce-e4b9c59e2969",
            "f2c477fb-28ea-4fcb-943a-9fab22df3da0",
            "7c5ae357-e079-4427-a90f-97d164c7262e",
            "73265ee3-bb35-40d1-b696-1f241a6f5966",
            "db33a54c-3934-478f-bad4-fc313ac2580e"
          ],
          "bullpen": [
            "b390b28c-df96-443e-b81f-f0104bd37860",
            "0f62c20c-72d0-4c12-a9d7-312ea3d3bcd1",
            "23e78d92-ee2d-498a-a99c-f40bc4c5fe99",
            "f1185b20-7b4a-4ccc-a977-dc1afdfd4cb9",
            "9313e41c-3bf7-436d-8bdc-013d3a1ecdeb",
            "3be2c730-b351-43f7-a832-a5294fe8468f",
            "e749dc27-ca3b-456e-889c-d2ec02ac7f5f",
            "d97835fd-2e92-4698-8900-1f5abea0a3b6"
          ],
          "bench": [
            "26f01324-9d1c-470b-8eaa-1b9bfbcd8b65",
            "9f6d06d6-c616-4599-996b-ec4eefcff8b8",
            "0e27df51-ad0c-4546-acf5-96b3cb4d7501"
          ],
          "seasAttr": [],
          "permAttr": [],
          "fullName": "San Francisco Lovers",
          "location": "San Francisco",
          "mainColor": "#780018",
          "nickname": "Lovers",
          "secondaryColor": "#212121",
          "shorthand": "SFL",
          "emoji": "0x1F48B",
          "slogan": "Let's Go All The Way!",
          "shameRuns": 0,
          "totalShames": 24,
          "totalShamings": 8,
          "seasonShames": 4,
          "seasonShamings": 5,
          "championships": 0,
          "weekAttr": [],
          "gameAttr": []
        },
        // ... 19 other team objects ...
      ],
      "subleagues": [
        {
          "id": "7d3a3dd6-9ea1-4535-9d91-bde875c85e80",
          "divisions": [
            "f711d960-dc28-4ae2-9249-e1f320fec7d7",
            "5eb2271a-3e49-48dc-b002-9cb615288836"
          ],
          "name": "The Good League"
        },
        {
          "id": "93e58443-9617-44d4-8561-e254a1dbd450",
          "divisions": [
            "765a1e03-4101-4e8e-b611-389e71d13619",
            "7fbad33c-59ab-4e80-ba63-347177edaa2e"
          ],
          "name": "The Evil League"
        }
      ],
      "divisions": [
        {
          "id": "f711d960-dc28-4ae2-9249-e1f320fec7d7",
          "teams": [
            "b72f3061-f573-40d7-832a-5ad475bd7909",
            "878c1bf6-0d21-4659-bfee-916c8314d69c",
            "b024e975-1c4a-4575-8936-a3754a08806a",
            "adc5b394-8f76-416d-9ce9-813706877b84",
            "ca3f1c8c-c025-4d8e-8eef-5be6accbeb16"
          ],
          "name": "Lawful Good"
        },
        {
          "id": "5eb2271a-3e49-48dc-b002-9cb615288836",
          "teams": [
            "bfd38797-8404-4b38-8b82-341da28b1f83",
            "3f8bbb15-61c0-4e3f-8e4a-907a5fb1565e",
            "979aee4a-6d80-4863-bf1c-ee1a78e06024",
            "7966eb04-efcc-499b-8f03-d13916330531",
            "36569151-a2fb-43c1-9df7-2df512424c82"
          ],
          "name": "Chaotic Good"
        },
        {
          "id": "765a1e03-4101-4e8e-b611-389e71d13619",
          "teams": [
            "8d87c468-699a-47a8-b40d-cfb73a5660ad",
            "23e4cbc1-e9cd-47fa-a35b-bfa06f726cb7",
            "f02aeae2-5e6a-4098-9842-02d2273f25c7",
            "57ec08cc-0411-4643-b304-0e80dbc15ac7",
            "747b8e4a-7e50-4638-a973-ea7950a3e739"
          ],
          "name": "Lawful Evil"
        },
        {
          "id": "7fbad33c-59ab-4e80-ba63-347177edaa2e",
          "teams": [
            "eb67ae5e-c4bf-46ca-bbbc-425cd34182ff",
            "9debc64f-74b7-4ae1-a4d6-fce0144b6ea5",
            "b63be8c2-576a-4d6e-8daf-814f8bcea96f",
            "105bc3ff-1320-4e37-8ef0-8d595cb95dd0",
            "a37f9158-7f82-46bc-908c-c9e2dda7c33b"
          ],
          "name": "Chaotic Evil"
        }
      ],
      "leagues": [
        {
          "id": "d8545021-e9fc-48a3-af74-48685950a183",
          "subleagues": [
            "7d3a3dd6-9ea1-4535-9d91-bde875c85e80",
            "93e58443-9617-44d4-8561-e254a1dbd450"
          ],
          "name": "Internet League Blaseball",
          "tiebreakers": "72a618ed-c61c-4162-a455-3959a2d0e738"
        }
      ]
    },
    "temporal": {
      "doc": {
        "id": "whatistime",
        "alpha": 1000,
        "beta": 1,
        "gamma": 500000000,
        "delta": true,
        "epsilon": false,
        "zeta": "WHERE IS YOUR FAITH"
      }
    }
  }
}
```
