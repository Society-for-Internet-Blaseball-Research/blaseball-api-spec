# Election Details

List of decrees and blessings for the end of the current season

## Endpoint

`https://www.blaseball.com/database/offseasonSetup`

## Response

```json
{
  "decrees": [
    {
      "id": "fifth_base",
      "type": 28,
      "title": "Fifth Base",
      "description": "The Top 4 Teams of the Regular Season must run an extra base next season."
    },
    {
      "id": "walk_in_the_park",
      "type": 29,
      "title": "Walk in the Park",
      "description": "The Top 4 Teams of the Regular Season will walk batters on the 3rd Ball of an At-Bat instead of the 4th next season."
    }
  ],
  "blessings": [
    {
      "id": "steal_random_leaderboard_player",
      "type": 87,
      "value": 1,
      "title": "Popular by Association",
      "subheader": "Brought to you by @The Multitude Podcast Collective@http://multitude.productions/blaseball",
      "description": "OMG they noticed us. Steal a random player from the Idol Leaderboard."
    },
    {
      "id": "item_fireproof",
      "type": 62,
      "value": 1,
      "title": "Scorpler's Jacket",
      "description": "Armor. Protect a random Player on your team from Incinerations."
    }
  ],
  "decreesToPass": 1
}
```

## Field Descriptions

**`decrees`**: List of decrees.

**`decrees.id`**: The text ID of the decree.

**`decrees.type`**: The integer ID of the decree.

**`decrees.title`**: The title displayed in the election page.

**`decrees.description`**: What will happen if this decree is enacted.

**`blessings`**: List of blessings.

**`blessings.id`**: The text ID of the blessing.

**`blessings.type`**: The integer ID of the blessing.

**`blessings.value`**: Unknown

**`blessings.title`**: The title displayed in the election page.

**`blessings.subheader`**: The sponsor's name and website link for sponsored blessings. (optional)

**`blessings.description`**: What will happen from this blessing.

**`decreesToPass`**: How many decrees will take effect.
