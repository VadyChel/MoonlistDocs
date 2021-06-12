# Overview

## Versions
| Name  | Url                                                | Status |
| ----- | -------------------------------------------------- | ------ |
| v1    | [api.moonlist.xyz/v1](https://api.moonlist.xyz/v1) | active |

## Important
- ? after the field type means that the field is optional

## Discord User Model
| Field         | Type      | Description |
| ------------- | --------- | ------ |
| id            | snowflake | active |
| bot           | boolean   | active |
| username      | string    | active |
| avatar        | string?   | active |
| discriminator | integer   | active |
| public_flags  | integer   | active |

### Example

```json
{
  "id": "660110922865704980",
  "bot": false,
  "username": "Vython.lui",
  "avatar": null,
  "discriminator": 9339,
  "public_flags": 0
}
```

## Discord Emoji Model
| Field    | Type    | Description |
| -------- | ------- | ------ |
| id       | string  | active |
| name     | string  | active |
| animated | boolean | active |

### Example

```json
{
  "id": "816231004422668298",
  "animated": false,
  "name": "morda"
}
```

## Discord Guild Model
| Field                      | Type                 | Description |
| -------------------------- | -------------------- | ------ |
| id                         | snowflake            | active |
| name                       | string               | active |
| icon                       | string?              | active |
| region                     | string               | active |
| banner                     | string?              | active |
| approximate_member_count   | integer              | active |
| approximate_presence_count | integer              | active |
| emojis                     | List[DiscordEmoji]   | active |

### Example

```json
{
  "id": "814563717710741534",
  "region": "europe",
  "name": "Moonlist Community",
  "icon": null,
  "approximate_member_count": 56,
  "approximate_presence_count": 23,
  "emojis": [],
  "banner": null
}
```