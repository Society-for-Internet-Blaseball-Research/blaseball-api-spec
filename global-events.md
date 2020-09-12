# Global Events

An array of messages that make up the content of the ticker at the top of the Blaseball site after logging in.

## Endpoint

`https://www.blaseball.com/database/globalEvents`

## Response

```json
[
  {
    "id": "the_discipline_era",
    "msg": "The Discipline Era has begun",
    "expire": null
  },
  {
    "id": "darkness_forecast",
    "msg": "THE COMMISSIONER IS DOING A GREAT JOB",
    "expire": null
  }
]
```

## Field Descriptions

**`id`**: The id of the given message.

**`msg`**: The message that is displayed in the ticker.

**`expires`**: Null for a semi-permenant message, or an ISO 8601 timestamp for when the message expires.
