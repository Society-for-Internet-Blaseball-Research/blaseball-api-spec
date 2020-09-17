# Election Details

List of decrees and blessings/bonuses for the end of the current season

## Endpoint

`https://www.blaseball.com/database/offseasonSetup`

## Response

```json
{
  "decrees": [
    {
      "id": "confuse_good",
      "type": 20,
      "title": "Confuse Good",
      "description": " "
    },
    {
      "id": "confuse_evil",
      "type": 21,
      "title": "Confuse Evil",
      "description": " "
    }
  ],
  "blessings": [
    {
      "id": "item_fireproof",
      "type": 62,
      "value": 1,
      "title": "Fireproof Jacket",
      "description": "Armor. Protect a random Player on your team from Incinerations."
    },
    {
      "id": "mod_team_soundproof",
      "type": 65,
      "value": 1,
      "title": "Wax",
      "description": "Your team is protected from Feedback for the following season."
    }
  ],
  "decreesToPass": 1
}
```

## Field Descriptions

**`decrees`**: List of decrees.

**`decrees.type`**: Integer ID of the decree.

**`decrees.title`**: The title displayed in the election page.

**`decrees.description`**: What will happen if this decree is enacted.

**`bonuses`**: List of bonuses

**`bonuses.type`**: Integer ID of the bonus.

**`bonuses.value`**: Unknown

**`bonuses.title`**: The title displayed in the election page.

**`bonuses.description`**: What will happen from this bonus.

**`decreesToPass`**: How many decrees will take effect
