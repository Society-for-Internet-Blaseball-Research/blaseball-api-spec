# Decree Results

What happened as the result of a specific decree.

## Endpoint

`https://blaseball.com/database/decreeResults?ids=:id1,id2,...`

## Response

```json
[
    {
        "_id": "49f975c9-eeb5-46e0-9cb6-6908695f7145",
        "decreeId": "four_for_four",
        "decreeTitle": "The Fourth Strike",
        "description": "The Four teams are chosen.\nThe Fourth Strike is granted to the New York Millennials\nThe Fourth Strike is granted to the Kansas City Breath Mints\nThe Fourth Strike is granted to the Hellmouth Sunbeams\nThe Fourth Strike is granted to the San Francisco Lovers\nMay the Fourth Strike save them all.",
        "totalVotes": 3028
    },
    {
        "_id": "59e1a46b-bc82-42f2-b8bb-be1b751e49a2",
        "decreeId": "peanuts",
        "decreeTitle": "Peanuts",
        "description": "Peanuts. Get Your Peanuts.",
        "totalVotes": 4441
    }
]
```

## Field Descriptions

**`decreeId`**: The name id of the decree.

**`decreeTitle`**: The title displayed on the elections page.

**`description`**: The description for this decree on the elections page.

**`totalVotes`**: How many votes this decree got.