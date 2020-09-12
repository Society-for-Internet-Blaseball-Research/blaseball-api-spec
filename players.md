# Players 

Get individual stats for one or more players. Returns an array. Use commas to separate multiple player IDs.

## Endpoint

`https://www.blaseball.com/database/players?ids=:id1,:id2,...`

## Response

```json
[
    {
        "id": "17397256-c28c-4cad-85f2-a21768c66e67",
        "name": "Cory Ross",
        "deceased": false,
        "peanutAllergy": true,
        
        "baseThirst": 0.8163297863171528,
        "continuation": 0.9332406398132362,
        "groundFriction": 0.6234756539195374,
        "indulgence": 0.6302776113973703,
        "laserlikeness": 0.5813163393413376,

        "anticapitalism": 0.3865984034527832,
        "chasiness": 0.3876884722913716,
        "omniscience": 0.40240204027262094,
        "tenaciousness": 0.5321892387925751,
        "watchfulness": 0.6211609170901324,
        
        "buoyancy": 0.7295030935858079,
        "divinity": 0.865859860942711,
        "martyrdom": 0.8183643543823621,
        "moxie": 0.9930963701536112,
        "musclitude": 0.5244697447949057,
        "patheticism": 0.7852546298408897,
        "thwackability": 0.1337877991334099,
        "tragicness": 0.1,
        
        "coldness": 0.04077503022645801,
        "overpowerment": 0.588492025671367,
        "ruthlessness": 0.034373471563752256,
        "shakespearianism": 0.4707237610843995,
        "suppression": 0.7581323899020682,
        "unthwackability": 0.46406385877539,
        "totalFingers": 10,
        
        "cinnamon": 0.30903546718079355,
        "pressurization": 0.19961729034104736,
        "soul": 6,
        "bat": "",
        "fate": 32
    }
]
```

## Field Descriptions

**`id`**: The ID of the player.

**`name`**: The player's name.

**`deceased`**: Whether the player is dead or not.

**`peanutAllergy`**: Whether or not this player has a peanut allergy. (Added in Season 3)

### Baserunning Attributes

**`baseThirst`**: Unknown

**`continuation`**: Unknown

**`groundFriction`**: Unknown

**`indulgence`**: Unknown

**`laserlikeness`**: Unknown

### Defense Attributes

**`anticapitalism`**: Unknown

**`chasiness`**: Unknown

**`omniscience`**: Unknown

**`tenaciousness`**: Unknown

**`watchfulness`**: Unknown

### Hitting Attributes

**`buoyancy`**: Unknown

**`divinity`**: Unknown

**`martyrdom`**: Unknown

**`moxie`**: Unknown

**`musclitude`**: Unknown

**`patheticism`**: Unknown

**`thwackability`**: Unknown

**`tragicness`**: Unknown

### Pitching Attributes

**`coldness`**: Unknown

**`overpowerment`**: Unknown

**`ruthlessness`**: Unknown

**`shakespearianism`**: Unknown

**`suppression`**: Unknown

**`unthwackability`**: Unknown

**`totalFingers`**: The number of fingers the player has.

### Other Attributes

**`cinnamon`**: Unknown (Added in Season 3)

**`pressurization`**: Unknown

**`soul`**: Unknown

**`bat`**: The name of the player's bat, if any. (Added in Season 3)

**`fate`**: Unknown (Added in Season 3)
