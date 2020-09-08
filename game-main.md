# Game Object Details

There are currently 4 different endpoints that return game objects, this page serves as a central place to define what is in a game object.


## Sample Game Object

```json
{
  "id": "dc767612-eb77-417b-8d2f-c21eb4dab868",
  "basesOccupied": [],
  "baseRunners": [],
  "baseRunnerNames": [],
  "baserunnerCount": 0,
  "outcomes": [],
  "terminology": "b67e9bbb-1495-4e1b-b517-f1444b0a6c8b",
  "lastUpdate": "Game over.",
  "rules": "4ae9d46a-5408-460a-84fb-cbd8d03fff6c",
  "statsheet": "a8fd2115-7d95-42f9-8bfe-b44132da2b16",
  "awayPitcher": "c182f33c-aea5-48a2-97ed-dc74fa29b3c0",
  "awayPitcherName": "Swamuel Mora",
  "awayBatter": "e4e4c17d-8128-4704-9e04-f244d4573c4d",
  "awayBatterName": "Wesley Poole",
  "awayTeam": "ca3f1c8c-c025-4d8e-8eef-5be6accbeb16",
  "awayTeamName": "Chicago Firefighters",
  "awayTeamNickname": "Firefighters",
  "awayTeamColor": "#8c2a3e",
  "awayTeamEmoji": "0x1F525",
  "awayOdds": 0.5583847767978104,
  "awayStrikes": 3,
  "awayScore": 4,
  "awayTeamBatterCount": 35,
  "homePitcher": "db33a54c-3934-478f-bad4-fc313ac2580e",
  "homePitcherName": "Percival Wheeler",
  "homeBatter": null,
  "homeBatterName": null,
  "homeTeam": "b72f3061-f573-40d7-832a-5ad475bd7909",
  "homeTeamName": "San Francisco Lovers",
  "homeTeamNickname": "Lovers",
  "homeTeamColor": "#780018",
  "homeTeamEmoji": "0x1F48B",
  "homeOdds": 0.44161522320218954,
  "homeStrikes": 3,
  "homeScore": 2,
  "homeTeamBatterCount": 31,
  "season": 1,
  "isPostseason": false,
  "day": 28,
  "phase": 4,
  "gameComplete": true,
  "finalized": true,
  "gameStart": true,
  "halfInningOuts": 0,
  "halfInningScore": 0,
  "inning": 8,
  "topOfInning": false,
  "atBatBalls": 0,
  "atBatStrikes": 0,
  "seriesIndex": 2,
  "seriesLength": 3,
  "shame": false,
  "weather": 7
}
```

## Field Descriptions

**`id`**: The ID of the game.

**`basesOccupied`**: A list of bases with runners on them. Bases are zero indexed with `0` being first base, `1` being second base, and `2` being third base.

**`baseRunners`**: A list of IDs of the players on bases. Believed to be in order or at least the same order as `basesOccupied`.

**`baseRunnerNames`**: A list of names of the players on bases. Believed to be in order or at least the same order as `basesOccupied`.

**`baserunnerCount`**: The number of runners currently on bases.

**`outcomes`**: A list of strings corresponding to weather related events that happened this game. Currently known events include things like incineration, peanut reactions, feedback swaps, and reverb. The array is populated at the time of the event and stays populated through the end of the game.

**`terminology`**: The ID of the terminology for the game. Unknown what this ID goes to.

**`lastUpdate`**: The text for the update as displayed in the live game box.

**`rules`**: The ID of the rules for the game. Unknown what this ID goes to.

**`statsheet`**: The ID of the statsheet for the game. Goes to the [game statsheet](game-statsheet.md) endpoint.

**`awayPitcher`**: The ID of the current pitcher for the away team.

**`awayPitcherName`**: The name of the current pitcher for the away team.

**`awayBatter`**: The ID of the current battter for the away team.

**`awayBatterName`**: The name of the current batter for the away team.

**`awayteam`**: The ID of the away team.

**`awayTeamName`**: The name of the away team.

**`awayTeamNickname`**: The nickname of the away team.

**`awayTeamColor`**: The hex color code of the away team.

**`awayTeamEmoji`**: The codepoint for the team emoji

**`awayOdds`**: The odds for this game of the away team winning.

**`awayStrikes`**: The number of strikes it takes to strike out a player from the away team.

**`awayScore`**: The current score of the away team.

**`awayTeamBatterCount`**: The current index of the total batter list for the game for the away team (zero indexed). 

**`homePitcher`**: The ID of the current pitcher for the home team.

**`homePitcherName`**: The name of the current pitcher for the home team.

**`homeBatter`**: The ID of the current battter for the home team.

**`homeBatterName`**: The name of the current batter for the home team.

**`hometeam`**: The ID of the home team.

**`homeTeamName`**: The name of the home team.

**`homeTeamNickname`**: The nickname of the home team.

**`homeTeamColor`**: The hex color code of the home team.

**`homeTeamEmoji`**: The codepoint for the team emoji

**`homeOdds`**: The odds for the game of the home team winning.

**`homeStrikes`**: The number of strikes it takes to strike out a player from the home team.

**`homeScore`**: The current score of the home team.

**`homeTeamBatterCount`**: The current index of the total batter list for the game for the home team (zero indexed). 

**`season`**: The season (zero indexed) that the game belongs to.

**`isPostSeason`**: A boolean indicating if the game is in the postseason.

**`day`**: The day (zero indexed) that the game is happening on.

**`phase`**: An integer indicating something likely related to site state, not much is known for sure.

**`gameComplete`**: A boolean indicating whether or not the game has finished.

**`finalized`**: A boolean indicating whether or not the game is "finalized". What exactly this means is not currently clear.

**`gameStart`**: A boolean indicating whether or not the game has started.

**`halfInningOuts`**: The number of outs for the current half-inning.

**`halfInningScore`**: The number of runs scored for the current half-inning.

**`inning`**: The current inning (zero indexed).

**`topOfInning`**: A boolean indicating whether or not it is currently the top of the inning.

**`atBatBalls`**: The number of balls for the current at-bat.

**`atBatStrikes`**: The number of strikes for the current at-bat.

**`seriesIndex`**: The current index (1 indexed) of the game in the series.

**`seriesLength`**: The length of the current series.

**`shame`**: A boolean indicating whether or not the game has entered or finished in shame.

**`weather`**: An integer representing the weather for the game. Mapping defined below:

| Number  | Weather  | Seen |
| -- | ------------- | ---- |
| 0  | Void          | No   |
| 1  | Sunny         | Yes  |
| 2  | Overcast      | No   |
| 3  | Rainy         | No   |
| 4  | Sandstorm     | No   |
| 5  | Snowy         | No   |
| 6  | Acidic        | No   |
| 7  | Solar Eclipse | Yes  |
| 8  | Glitter       | No   |
| 9  | Bloodwind     | No   |
| 10 | Peanuts       | Yes  |
| 11 | Bird          | Yes  |
| 12 | Feedback      | Yes  |
| 13 | Reverb        | Yes  |