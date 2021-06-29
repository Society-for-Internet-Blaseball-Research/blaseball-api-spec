# Shop Setup (Concessions)

Information on available concessions as well as costs and associated values for snacks which can be purchased multiple times.

## Endpoint

`https://blaseball.com/database/shopSetup`

## Response

```json
{
  "menu": [
    "Ad",
    "Votes",
	/* ... */
    "Idol_Pitcher_Loss",
    "Consumer_Attacks"
  ],
  "snackData": {
    "maxBetTiers": [ /* array of 99 price/amount pairs */ ],
    "teamWinCoinTiers": [ /* array of 99 price/amount pairs */ ],
    "idolHitsTiers": [ /* array of 99 price/amount pairs */ ],
    "idolHomersTiers": [ /* array of 99 price/amount pairs */ ],
    "idolStrikeoutsTiers": [ /* array of 99 price/amount pairs */ ],
    "idolShutoutsTiers": [ /* array of 99 price/amount pairs */ ],
    "teamLossCoinTiers": [ /* array of 99 price/amount pairs */ ],
    "idolStealTiers": [ /* array of 99 price/amount pairs */ ],
    "blackHoleTiers": [ /* array of 99 price/amount pairs */ ],
    "floodClearTiers": [ /* array of 99 price/amount pairs */ ],
    "idolHomerAllowedTiers": [ /* array of 99 price/amount pairs */ ],
    "timeOffTiers": [ /* array of 99 price/amount pairs */ ],
    "sunTwoTiers": [ /* array of 99 price/amount pairs */ ],
    "idolPitcherWinTiers": [ /* array of 99 price/amount pairs */ ],
    "idolPitcherLoseTiers": [ /* array of 99 price/amount pairs */ ],
    "teamShamedTiers": [ /* array of 99 price/amount pairs */ ],
    "teamShamingTiers": [ /* array of 99 price/amount pairs */ ],
    "incinerationTiers": [ /* array of 99 price/amount pairs */ ],
    "consumerTiers": [ /* array of 99 price/amount pairs */ ],
  }
}
```

The price/amount pairs are an array of 99 objects in the form `{"price":1234,"amount":5678}`. For example, the first and last few entries for `maxBetTiers` (Snake Oil) are:

```json
{ "price": 0, "amount": 20 },
{ "price": 20, "amount": 40 },
/* 95 entries omitted */
{ "price": 9845, "amount": 1980 },
{ "price": 10000, "amount": 2000 }
	
```

## Field Descriptions

**`menu`**: array of strings corresponding to snacks currently available in Concessions as well as the sponsor advertisement shown when entering the shop. They are not in the same order that the're displayed in the shop. (Correlations are currently guesses.)

- `Ad` - The sponsor's advertisement; not really for sale
- `Votes` - Vote
- `Flutes` - Flutes
- `Beg` - Bread Crumbs
- `Peanuts` - Peanuts
- `Max_Bet` - Snake Oil
- `Team_Win` - Popcorn
- `Idol_Strikeouts` - Chips
- `Idol_Shutouts` - Burger
- `Idol_Homers` - Hot Dog
- `Idol_Hits` - Sunflower Seeds
- `Team_Loss` - Stale Popcorn
- `Stadium_Access` - Pizza 
- `Wills_Access` - Cheese Board
- `Forbidden_Knowledge_Access` -  Apple(?)
- `Idol_Steal` - Pickles
- `Black_Hole` - Wet Pretzel
- `Team_Slush` - Slushie(?)
- `Sun_2` - Doughnut
- `Idol_Homer_Allowed` - Meatball
- `Breakfast` - Breakfast
- `Incineration` - Sundae
- `Idol_Pitcher_Win` - Hot Fries
- `Idol_Pitcher_Loss` - Cold Fries
- `Consumer_Attacks` - Chum

**`snackData`**: Pricing and value information for snacks. This is an array corresponding with own 1 through 99 of a given snack. Each array item is an object with two values: `"price"` and `"amount"`.  The `price` is the cost to acquire the next number of that snack, the amount is the associated value (ex: maximum bet for maxBetTiers/Snake Oil, coins for each base stolen for idealStealTiers/Pickles).

- `maxBetTiers` - Snake Oil
- `teamWinCoinTiers` - Popcorn
- `idolHitsTiers` - Sunflower Seeds
- `idolHomersTiers` - Hot Dog
- `idolStrikeoutsTiers` - Chips
- `idolShutoutsTiers` - Burger
- `teamLossCoinTiers` - Stale Popcorn
- `idolStealTiers` - Pickles
- `blackHoleTiers` - Wet Pretzel
- `floodClearTiers` - Slushie
- `idolHomerAllowedTiers` - Meatball
- `timeOffTiers` - Breakfast
- `sunTwoTiers` - Doughnut
- `idolPitcherWinTiers` - Hot Fries
- `idolPitcherLoseTiers` - Close Fries
- `teamShamedTiers` - Lemonade (retired)
- `teamShamingTiers` - Taffy (retired)
- `incinerationTiers` - Sundae
- `consumerTiers` - Chum


For example, the `maxBetTiers` first two and last two snackData objects are:

```json
{ "price": 0, "amount": 20 },
{ "price": 20, "amount": 40 },
/* 95 entries omitted */
{ "price": 9845, "amount": 1980 },
{ "price": 10000, "amount": 2000 }
```

This corresponds to owning 1 Snake Oil (Free, can bet up to 20), 2 Snake Oils (costs 20, can bet up to 40), 98 Snake Oils (costs 9,845, can bet up to 1980), and 99 Snake Oils (costs 10,000, can bet up to 2,000).
