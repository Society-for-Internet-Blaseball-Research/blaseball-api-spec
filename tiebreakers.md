# Tiebreaker Details

Returns inforation for a given tiebreaker ID from the league object. Each of the ids in `order` is an ID for a team object. This represents the "Divine Favor" ranking. (Note: the tiebreaker object is returned inside a single-element array, even though the endpoint's argument only accepts one ID.)

## Endpoint

`https://www.blaseball.com/database/tiebreakers?id=:tiebreaker_id`

## Response

```json
[
  {
    "id": "72a618ed-c61c-4162-a455-3959a2d0e738",
    "order": [
      "23e4cbc1-e9cd-47fa-a35b-bfa06f726cb7",
      "b72f3061-f573-40d7-832a-5ad475bd7909",
      "878c1bf6-0d21-4659-bfee-916c8314d69c",
      "b024e975-1c4a-4575-8936-a3754a08806a",
      "adc5b394-8f76-416d-9ce9-813706877b84",
      "ca3f1c8c-c025-4d8e-8eef-5be6accbeb16",
      "bfd38797-8404-4b38-8b82-341da28b1f83",
      "3f8bbb15-61c0-4e3f-8e4a-907a5fb1565e",
      "979aee4a-6d80-4863-bf1c-ee1a78e06024",
      "7966eb04-efcc-499b-8f03-d13916330531",
      "36569151-a2fb-43c1-9df7-2df512424c82",
      "8d87c468-699a-47a8-b40d-cfb73a5660ad",
      "f02aeae2-5e6a-4098-9842-02d2273f25c7",
      "57ec08cc-0411-4643-b304-0e80dbc15ac7",
      "747b8e4a-7e50-4638-a973-ea7950a3e739",
      "eb67ae5e-c4bf-46ca-bbbc-425cd34182ff",
      "9debc64f-74b7-4ae1-a4d6-fce0144b6ea5",
      "b63be8c2-576a-4d6e-8daf-814f8bcea96f",
      "105bc3ff-1320-4e37-8ef0-8d595cb95dd0",
      "a37f9158-7f82-46bc-908c-c9e2dda7c33b"
    ]
  }
]
```

## Field Descriptions

**`id`**: The ID of the tiebreaker object.

**`order`**: An array of team IDs in order of their tiebreaker favor.
