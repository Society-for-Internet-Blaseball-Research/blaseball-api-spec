# Standings Details

Returns inforation for a given standings id from the season object.

## Endpoint

`https://www.blaseball.com/database/standings?id=:standings_id`

## Response

```json
{
  "id": "48789741-69b1-4aa9-a46c-eda3351a3f5e",
  "losses": {
    "b72f3061-f573-40d7-832a-5ad475bd7909": 25,
    "878c1bf6-0d21-4659-bfee-916c8314d69c": 56,
    "b024e975-1c4a-4575-8936-a3754a08806a": 36,
    "adc5b394-8f76-416d-9ce9-813706877b84": 35,
    "ca3f1c8c-c025-4d8e-8eef-5be6accbeb16": 31,
    "bfd38797-8404-4b38-8b82-341da28b1f83": 39,
    "3f8bbb15-61c0-4e3f-8e4a-907a5fb1565e": 41,
    "979aee4a-6d80-4863-bf1c-ee1a78e06024": 36,
    "7966eb04-efcc-499b-8f03-d13916330531": 41,
    "36569151-a2fb-43c1-9df7-2df512424c82": 30,
    "8d87c468-699a-47a8-b40d-cfb73a5660ad": 24,
    "23e4cbc1-e9cd-47fa-a35b-bfa06f726cb7": 39,
    "f02aeae2-5e6a-4098-9842-02d2273f25c7": 45,
    "57ec08cc-0411-4643-b304-0e80dbc15ac7": 39,
    "747b8e4a-7e50-4638-a973-ea7950a3e739": 31,
    "eb67ae5e-c4bf-46ca-bbbc-425cd34182ff": 31,
    "9debc64f-74b7-4ae1-a4d6-fce0144b6ea5": 43,
    "b63be8c2-576a-4d6e-8daf-814f8bcea96f": 43,
    "105bc3ff-1320-4e37-8ef0-8d595cb95dd0": 39,
    "a37f9158-7f82-46bc-908c-c9e2dda7c33b": 26
  },
  "wins": {
    "b72f3061-f573-40d7-832a-5ad475bd7909": 48,
    "878c1bf6-0d21-4659-bfee-916c8314d69c": 17,
    "b024e975-1c4a-4575-8936-a3754a08806a": 37,
    "adc5b394-8f76-416d-9ce9-813706877b84": 38,
    "ca3f1c8c-c025-4d8e-8eef-5be6accbeb16": 42,
    "bfd38797-8404-4b38-8b82-341da28b1f83": 34,
    "3f8bbb15-61c0-4e3f-8e4a-907a5fb1565e": 32,
    "979aee4a-6d80-4863-bf1c-ee1a78e06024": 37,
    "7966eb04-efcc-499b-8f03-d13916330531": 32,
    "36569151-a2fb-43c1-9df7-2df512424c82": 43,
    "8d87c468-699a-47a8-b40d-cfb73a5660ad": 49,
    "23e4cbc1-e9cd-47fa-a35b-bfa06f726cb7": 34,
    "f02aeae2-5e6a-4098-9842-02d2273f25c7": 28,
    "57ec08cc-0411-4643-b304-0e80dbc15ac7": 34,
    "747b8e4a-7e50-4638-a973-ea7950a3e739": 42,
    "eb67ae5e-c4bf-46ca-bbbc-425cd34182ff": 42,
    "9debc64f-74b7-4ae1-a4d6-fce0144b6ea5": 30,
    "b63be8c2-576a-4d6e-8daf-814f8bcea96f": 30,
    "105bc3ff-1320-4e37-8ef0-8d595cb95dd0": 34,
    "a37f9158-7f82-46bc-908c-c9e2dda7c33b": 47
  }
}
```

## Field Descriptions

**`id`**: The ID of the standings object.

**`losses`**: An array of team IDs and how many losses each team has.

**`wins`**: An array of team IDs and how many wins each team has.
