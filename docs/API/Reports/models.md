## Report Model

| Field      | Type          | Description |
| ---------- | ------------- | ----------- |
| id         | `integer`     | asda |
| author_id  | `snowflake`   | asfasf |
| entity_id  | `snowflake`   | asfga |
| state      | `integer`     | agfas |
| created_at | `datetime`    | agfafa |
| reason     | `string`      | sfs asf |
| type       | `string`      | faa 
| author     | `DiscordUser` |

### Example
```json
{
  "id": 0,
  "author_id": "660110922865704980",
  "entity_id": "813065963003052073",
  "state": 0,
  "created_at": "2021-01-01T20:20:00.000000",
  "reason": "This is a report reason",
  "type": "bot",
  "author": {
      "id": "660110922865704980",
      "bot": false,
      "username": "Vython.lui",
      "avatar": null,
      "discriminator": 9339,
      "public_flags": 0
  }
}
```