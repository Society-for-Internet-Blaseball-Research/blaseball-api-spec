# Playoff Round

Information about a specific round in the playoffs.

## Endpoint

`https://www.blaseball.com/database/playoffRound?id=:id`

## Response

```json
{
    "id": "aecb79df-5f61-40c1-a244-8a42268f2e4c",
    "matchups": [
        "6bd6170f-7383-4d0f-845e-32ec9e934abd",
        "05f17a40-b999-4411-9a48-ee309f80ac28",
        "39f6e865-73e5-46c3-b9a9-3e846e7898db",
        "7cc52df5-1e20-417b-9915-cd62c534182a"
    ],
    "games": [
        [
            "c0080509-f1f6-4b86-9c31-88abf157e283",
            "c8c555e9-dfe7-46df-a56a-00eccfc2bb48",
            "b323e8e6-1e21-45cf-ac55-a634ce620cc4",
            "3bd61253-0972-4fa6-9bbc-4f0b8b202cdf",
            "none",
            "none",
            "none",
            "none"
        ],
        [
            "e8a22326-7c0a-4de2-bf97-dceea9f53edb",
            "164dcbb1-bc05-4cde-8853-01e0bd1f9cb0",
            "86ffa243-7910-4688-995d-1cdf8feccc2b",
            "5ebb73d3-8474-48a2-bb69-a28f97fa65e4"
        ],
        [
            "d76ddb03-b6f5-43cf-ac47-c77028182a1e",
            "d2577acd-2e1f-4eaf-90b8-9a509c7e5bd8",
            "195af1c6-8f82-4099-ac24-a64b6b1ba3e2",
            "8414e9cb-8a49-4722-b747-4748e18f8e53"
        ],
        [
            "fabe1105-58b3-47c4-8bce-9d0824404141",
            "7e23e6d3-911e-45a6-87d2-3a2efbcbae6f",
            "952de7c0-5b17-4e8f-8b56-caf01025a6a7",
            "1d8bc613-0ad4-4551-9570-27857e5cac42"
        ],
        [
            "none",
            "none",
            "460297c0-85c8-4887-ad34-add272e71bae",
            "86d68a1c-4106-47f6-aca1-1b1abfcd0ef4"
        ]
    ],
    "winners": [
        "36569151-a2fb-43c1-9df7-2df512424c82",
        "b72f3061-f573-40d7-832a-5ad475bd7909",
        "747b8e4a-7e50-4638-a973-ea7950a3e739",
        "23e4cbc1-e9cd-47fa-a35b-bfa06f726cb7"
    ],
    "winnerSeeds": [
        0,
        2,
        0,
        1
    ],
    "gameIndex": 4,
    "name": "Round 1",
    "roundNumber": 0,
    "special": false
}
```

## Field Descriptions

**`id`**: The ID of the playoff round.

**`matchups`**: List of playoff matchup IDs. Can be looked up using the [playoff matchups](playoff-matchups.md) endpoint.

**`games`**: A list of lists of game IDs. Each sublist represents a day in the round with the games that each pair of teams played that day.

**`winners`**: Teams that won their matchups.

**`winnerSeeds`**: Seeds for the winners (sometimes negative?).

**`gameIndex`**: The number of games that have been played so far (zero indexed).

**`name`**: Round name.

**`roundNumber`**: Round number (zero indexed).

**`special`**: Currently seems to indicate final round of playoffs.
