# Divisions

Returns information for a given division ID.

## Endpoint

`https://www.blaseball.com/database/division?id=:division_id`

## Response

```json
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
}
```

## Field Descriptions

**`id`**: The ID of the division.

**`teams`**: An array of IDs for the teams that belong to the division.

**`name`**: The name of the division.
