# Game Object Details

There are currently 4 different endpoints that return game objects, this page serves as a central place to define what is in a game object.


## Sample Game Object

```json
{
  "id":"aac86d9c-68c3-4a00-8d34-850458d79a0c",
"basesOccupied":[],
"baseRunners":[],
"baseRunnerNames":[],
"outcomes":[],
"terminology":"b67e9bbb-1495-4e1b-b517-f1444b0a6c8b",
"lastUpdate":"Lift 9,
 Worms 7",
"rules":"4ae9d46a-5408-460a-84fb-cbd8d03fff6c",
"statsheet":"320750ed-3fde-4ac8-8e5a-a077c0a4b072",
"awayPitcher":"ccd6068b-2735-4072-bfe5-571a5d57c285",
"awayPitcherName":"Ephraim Ladd",
"awayBatter":null,
"awayBatterName":"",
"awayTeam":"bb4a9de5-c924-4923-a0cb-9d1445f1ee5d",
"awayTeamName":"Ohio Worms",
"awayTeamNickname":"Worms",
"awayTeamColor":"#5c4822",
"awayTeamEmoji":"0x1F40C",
"awayOdds":0.4594541379293016,
"awayStrikes":3,
"awayScore":7,
"awayTeamBatterCount":36,
"homePitcher":"62ae6aa9-e346-4faa-b07c-1f7623580015",
"homePitcherName":"Gerund Pantheocide",
"homeBatter":null,
"homeBatterName":"",
"homeTeam":"c73b705c-40ad-4633-a6ed-d357ee2e2bcf",
"homeTeamName":"Tokyo Lift",
"homeTeamNickname":"Lift",
"homeTeamColor":"#e830ab",
"homeTeamEmoji":"🏋️‍♀️",
"homeOdds":0.5405458620706983,
"homeStrikes":3,
"homeScore":9,
"homeTeamBatterCount":46,
"season":12,
"isPostseason":false,
"day":0,
"phase":7,
"gameComplete":true,
"finalized":true,
"gameStart":true,
"halfInningOuts":0,
"halfInningScore":0,
"inning":8,
"topOfInning":true,
"atBatBalls":0,
"atBatStrikes":0,
"seriesIndex":1,
"seriesLength":3,
"shame":false,
"weather":11,
"baserunnerCount":0,
"homeBases":4,
"awayBases":4,
"repeatCount":0,
"awayTeamSecondaryColor":"#ba9c65",
"homeTeamSecondaryColor":"#e830ab",
"homeBalls":4,
"awayBalls":4,
"homeOuts":3,
"awayOuts":3,
"playCount":390,
"tournament":-1,
"baseRunnerMods":[],
"homePitcherMod":"",
"homeBatterMod":"",
"awayPitcherMod":"",
"awayBatterMod":"",
"scoreUpdate":"",
"scoreLedger":"",
"stadiumId":null,
"secretBaserunner":null,
"topInningScore":0,
"bottomInningScore":0,
"newInningPhase":-1,
"gameStartPhase":18,
"isTitleMatch":false

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
| 1  | Sun 2         | Yes  |
| 2  | Overcast      | No   |
| 3  | Rainy         | No   |
| 4  | Sandstorm     | No   |
| 5  | Snowy         | No   |
| 6  | Acidic        | No   |
| 7  | Solar Eclipse | Yes  |
| 8  | Glitter       | No   |
| 9  | Blooddrain    | Yes  |
| 10 | Peanuts       | Yes  |
| 11 | Lots of Birds | Yes  |
| 12 | Feedback      | Yes  |
| 13 | Reverb        | Yes  |
| 14 | Black Hole    | Yes  |
| 15 | Coffee        | Yes  |
| 16 | Coffee 2      | Yes  |
| 17 | Coffee 3s     | Yes  |
| 18 | Flooding      | Yes  |
| 19 | ???           | No   |
| 20 | ???           | No   |
| 21 | ???           | No   |
| 22 | ???           | No   |


**`homeBases`**: Number of bases the home team will run while batting

**`awayBases`**: Number of bases the away team will run while batting

**`repeatCount`**: ?

**`awayTeamSecondaryColor`**: An alternate color for the away team

**`homeTeamSecondaryColor`**: An alternate color for the home team

**`homeBalls`**: Number of balls per at bat for the home team

**`awayBalls`**: Number of balls per at bat for the away team

**`homeOuts`**: Number of outs per inning for the home team

**`awayOuts`**: Number of outs per inning for the away team

**`playCount`**: Number of plays in the game (updates)

**`tournament`**: a boolean indicating if this is a tournament game

**`baseRunnerMods`**: List of modifiers on the baserunners

**`homePitcherMod`**: Modifier on home pitcher

**`homeBatterMod`**: Modifier on home batter

**`awayPitcherMod`**: Modifier on away pitcher

**`awayBatterMod`**: Modifier on away batter

**`scoreUpdate`**: ?

**`scoreLedger`**: ?

**`stadiumId`**: Id of the stadium in which this game is played

**`secretBaserunner`**: ?

**`topInningScore`**: Score in the current or latest top half of inning

**`bottomInningScore`**: Score in the current or latest bottom half of inning

**`newInningPhase`**: ?

**`gameStartPhase`**: ?

**`isTitleMatch`**: A boolean indicating whether this game is a title match

