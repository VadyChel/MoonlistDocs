## Server Model

| Field             | Type         | Description |
| ----------------- | ------------ | ------ |
| id                | integer      | active |
| guild_id          | snowflake    | active |
| owner_id          | snowflake    | active |
| added_at          | datetime     | active |
| invite            | string       | active |
| short_description | string       | active |
| description       | string       | active |
| features          | Map          | active |
| tags              | List[string] | active |
| discord           | DiscordGuild | active |
| count_bumps       | integer      | active |

### Example
```json
{
    "id": 0,
    "guild_id": "814563717710741534",
    "owner_id": "660110922865704980",
    "added_at": "2021-01-01T20:20:00.000000",
    "invite": "uJJD7Deqyb",
    "short_description": "This is a short description",
    "description": "This is a long description",
    "features": {},
    "tags": ["CustomTag", "Tag1", "Economy"],
    "discord": {},
    "count_bumps": 56
}
```