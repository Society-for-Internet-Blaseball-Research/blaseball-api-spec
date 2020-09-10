# Single Season Statsheet

## Deprecated

**DO NOT USE THIS ENDPOINT**. Use the [season statsheet](season-statsheet.md) endpoint instead. This endpoint can only fetch the statsheet for a single season and using it repeatedly would cause unnecessary load on the Blaseball servers.

Get the statsheet for a single season.

## Endpoint

`https://www.blaseball.com/database/seasonStatsheet?id=:statsheetId`

## Response

```json
{
  "id": "64392ad5-e14c-42c0-825c-c85da29addaa",
  "teamStats": [
    "9298cca4-442e-4aa0-8bcf-8ee349b1a45e",
    "cc0fb608-945e-4b3f-8848-0c73dc6d32dc",
    "bc5646fd-e892-4bd7-8631-84ac402c9ac9",
    "9d06f0e1-d221-4e2e-8af1-6b9570fe3e71",
    "eee9264e-c902-45fa-b981-2a49da1b04d5",
    "0f587e43-fb3d-4a24-8a26-79ad99a612a6",
    "a66c2f35-084f-4fae-a31a-436a905861e8",
    "5e6fc1bd-d836-434f-aa28-c0e7298ca98d",
    "5c2d22e0-18a5-4555-b839-77dc1cd79785",
    "2232c53c-65cb-4941-99cb-8ed6969f2c62",
    "a7aefb4d-734d-4ca4-ad15-77f27ec808da",
    "206087b3-6e0a-4730-82ae-d708c1bec2ed",
    "096a5a7a-70a8-44d2-9349-7b283cf4f8a0",
    "5e03ef72-42a5-4014-8aa6-898cb9c55037",
    "666e094c-bf66-4efa-bf7a-e2131454c495",
    "787ce0a9-8789-4bf8-9887-51750b9753b4",
    "691ba727-6c87-4641-a706-c39a27e84fb5",
    "f013e9fa-f82d-4a51-b28c-ec07bdbc69dc",
    "664db604-7658-4c27-9287-a34981e90978",
    "397953e8-556d-4629-866c-3f1666f8dc49"
  ]
}
```

## Field Descriptions

**`id`**: The id for the season statsheet

**`teamStats`**: An array of IDs for each team's statsheet.