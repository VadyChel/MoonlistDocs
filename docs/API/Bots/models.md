## Bot Options Model

| Field          | Type      | Description |
| -------------- | --------- | ----------- |
| github         | `string?` | asda |
| website        | `string?` | asfasf |
| documentation  | `string?` | asfga |
| support_server | `string?` | agfas |

### Example
```json
{
  "github": "VadyChel/MoonlistBrain",
  "website": "https://brain.moonlist.xyz",
  "documentation": "https://docs.moonlist.xyz",
  "support_server": "uJJD7Deqyb"
}
```

## Bot Stat Custom Field Model

| Field | Type      | Description |
| ----- | --------- | ----------- |
| name  | `string`  | asda |
| count | `integer` | asfasf |

### Example
```json
{
  "name": "bandwidth",
  "count": 1
}
```

## Bot Stat Model

| Field             | Type                       | Description |
| ----------------- | -------------------------- | ----------- |
| id                | `integer`                  | asda |
| time              | `datetime`                 | asfasf |
| users             | `integer`                  | asfga |
| bot_id            | `snowflake`                | agfas |
| guilds            | `integer`                  | asda |
| shards            | `integer`                  | asfasf |
| memory_load       | `integer`                  | asfga |
| cpu_load          | `integer`                  | agfas |
| commands_executed | `integer`                  | asda |
| custom            | `List[BotStatCustomField]` | asfasf |


### Example
```json
{
  "id": 0,
  "time": "2021-01-01T20:20:00.000000",
  "users": 10000,
  "bot_id": "813065963003052073",
  "guilds": 200,
  "shards":  1,
  "memory_load": 2,
  "cpu_load": 1,
  "commands_executed": 100000,
  "custom":  [ 
    {
      "name": "bandwidth",
      "count": 1
    } 
  ]
}
```

## Bot Invite Model

| Field          | Type      | Default | Description 
| -------------- | --------- | ------- | ----------- |
| permissions    | `integer?`| 0  | asda   |
| slash_commands | `boolean?`| false   | asfasf |
| redirect_to    | `string?` | null    | asfga |

### Example
```json
{
  "permissions": 379968,
  "slash_commands": false,
  "redirect_to": null
}
```

## Bot Model

| Field             | Type                 | Description |
| ----------------- | -------------------- | ----------- |
| id                | `integer`            | asda |
| bot_id            | `snowflake`          | asfasf |
| count_bumps       | `integer`            | asfga |
| currently         | `integer`            | sagfas |
| added_at          | `datetime`           | agfafa |
| short_description | `string`             | sfs asf |
| description       | `string`             | faa 
| invite            | `BotInvite`          | faa 
| prefix            | `string`             | faa 
| tags              | `List[string]`       | faa 
| lib               | `string`             | faa 
| hidden            | `boolean`            | faa 
| pinned            | `boolean`            | faa 
| options           | `BotOptions`         | faa 
| badges            | `List[string]`       | faa 
| verificated       | `boolean`            | faa 
| stat              | `BotStat?`           | faa 
| discord           | `DiscordUser`        | faa 
| owner             | `DiscordUser`        | faa 
| owners            | `List[DiscordUser?]` | faa 

### Example
```json
{
  "id": 0,
  "bot_id": "813065963003052073",
  "count_bumps": 56,
  "currently": 2,
  "added_at": "2021-01-01T20:20:00.000000",
  "short_description": "This is a short description",
  "description": "This is a long description",
  "invite": {
      "permissions": 379968,
      "slash_commands": false,
      "redirect_to": null
    },
  "prefix": "mb.",
  "tags": ["CustomTag", "WebDashboard", "Information"],
  "lib": "discord.py",
  "hidden": false,
  "pinned": true,
  "options": {
      "github": "VadyChel/MoonlistBrain",
      "website": "https://brain.moonlist.xyz",
      "documentation": "https://docs.moonlist.xyz",
      "support_server": "uJJD7Deqyb"
    },
  "badges": [],
  "verificated": true,
  "stat?": {
      "id": 0,
      "time": "2021-01-01T20:20:00.000000",
      "users": 10000,
      "bot_id": "813065963003052073",
      "guilds": 200,
      "shards": 1,
      "memory_load": 2,
      "cpu_load": 1,
      "commands_executed": 100000,
      "custom":  [ 
          {
              "name": "bandwidth",
              "count": 1
          } 
      ]
  },
  "discord": {
      "id": "813065963003052073",
      "bot": true,
      "username": "Moonlist Brain",
      "avatar": null,
      "discriminator": 8544,
      "public_flags": 0
  },
  "owner": {
      "id": "660110922865704980",
      "bot": false,
      "username": "Vython.lui",
      "avatar": null,
      "discriminator": 9339,
      "public_flags": 0
  },
  "owners": []
}
```