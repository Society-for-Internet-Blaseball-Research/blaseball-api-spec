# Subleague Details

Returns information for a given subleague ID. Limited to a single subleague ID.

## Endpoint

`https://www.blaseball.com/database/subleague?id=:subleague_id`

## Response

```json
{
  "divisions": [
    "f711d960-dc28-4ae2-9249-e1f320fec7d7",
    "5eb2271a-3e49-48dc-b002-9cb615288836"
  ],
  "id":"7d3a3dd6-9ea1-4535-9d91-bde875c85e80",
  "name":"The Good League"
}
```

## Field Descriptions

**`divisions`**: The IDs of the divisions that belong to the subleague.

**`id`**: The ID of the subleague.

**`name`**: The name of the subleague.