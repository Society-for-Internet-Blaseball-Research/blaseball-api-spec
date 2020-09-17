# Decree Results

Get the results of one or more decrees. Returns an array. Use commas to separate multiple decree IDs.

## Endpoint

`https://www.blaseball.com/database/decreeResults?ids=:decree_id1,:decree_id2,...`

## Response

```json
[
    {
        "id": "49f975c9-eeb5-46e0-9cb6-6908695f7145",
        "decreeId": "four_for_four",
        "decreeTitle": "The Fourth Strike",
        "description": "The Four teams are chosen.\nThe Fourth Strike is granted to the New York Millennials\nThe Fourth Strike is granted to the Kansas City Breath Mints\nThe Fourth Strike is granted to the Hellmouth Sunbeams\nThe Fourth Strike is granted to the San Francisco Lovers\nMay the Fourth Strike save them all.",
        "totalVotes": 3028
    },
    {
        "id": "59e1a46b-bc82-42f2-b8bb-be1b751e49a2",
        "decreeId": "peanuts",
        "decreeTitle": "Peanuts",
        "description": "Peanuts. Get Your Peanuts.",
        "totalVotes": 4441
    }
]
```

## Field Descriptions

**`id`**: The hexadecimal ID of the decree.

**`decreeId`**: The name ID of the decree.

**`decreeTitle`**: The title displayed on the elections page.

**`description`**: The description for this decree on the elections page.

**`totalVotes`**: How many votes this decree got.
