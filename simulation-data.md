# Simulation Data

Get current data about the simulation, ie day, season, time to next cycle, etc

## Endpoint

`https://blaseball.com/database/simulationData

## Response

```json
{
    "id": "thisidisstaticyo",
        "day": 51,
        "league": "d8545021-e9fc-48a3-af74-48685950a183",
        "nextElectionEnd": "2020-09-20T19:15:00.295Z",
        "nextPhaseTime": "2020-09-14T16:00:00.678Z",
        "nextSeasonStart": "2020-09-21T16:00:00.295Z",
        "phase": 2,
        "playOffRound": 0,
        "playoffs": "f3118c69-63a2-434a-9724-bea36934b839",
        "rules": "4ae9d46a-5408-460a-84fb-cbd8d03fff6c",
        "season": 6,
        "seasonId": "554c7ce4-4c71-40d5-b05c-63e9bfd86601",
        "terminology": "b67e9bbb-1495-4e1b-b517-f1444b0a6c8b",
        "eraColor": "#ff0000",
        "eraTitle": "The Discipline Era",
        "twgo": "JHFMTOJMNPSMLMDGFOSEZDTMJWHPADAACGRTBBPBBCJRTPMJCSNKKAOMVMSTAJTVTCJIMPSSSTBFHRSSMSDKIRLWLVWSSMEIMCCDMDRTEIFBCLRMMW",
        "subEraColor": "#ffe082",
        "subEraTitle": "GETTING SHELLED",
        "attr": [
            "OPENED_BOOK",
            "UNLOCKED_PEANUTS",
            "EAT_THE_RICH",
            "UNLOCKED_INTERVIEWS",
            "UNLOCKED_IDOLS",
            "PARTY_TIME"
        ]
}
```

## Field Descriptions

**`id`**: this id is static yo.
**`day`**: current day, 0-indexed
**`league`**: league UUID
**`nextElectionEnd`**: UTC Datetime for when the current election cycle ends.
**`nextPhaseTime`**: UTC Datetime for when the simulation changes phase (ie next game day, transition from regular season to post season)
**`nextSeasonStart`**: UTC Datetime for when the next season starts.
**`phase`**: current simulation phase
**`playOffRound`**: Current playoff round. 0-indexed, defaults 0 during regular season.
**`playoffs`**: ID for current playoff object.
**`rules`**: TBD
**`season`**: current season, 0-indexed
**`seasonId`**: current season ID
**`terminology`**: TBD
**`eraColor`**: hex color value for era text.
**`eraTitle`**: string name of the era.
**`twgo`**: initials of every player that's gotten out. RIV.
**`subEraColor`**: hex color value for sub era text.
**`subEraTitle`**: string name of the sub era.
**`attr`**: string identifiers of simulation attributes (ie due to voting decrees)
