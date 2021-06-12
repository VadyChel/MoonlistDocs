## User Social Model

| Field     | Type      | Description |
| --------- | --------- | ----------- |
| github    | `string?` | asda |
| website   | `string?` | asfasf |
| youtube   | `string?` | sagfas |
| discord   | `string?` | agfafa |
| twitter   | `string?` | sfs asf |
| vk        | `string?` | faa 
| instagram | `string?` | faa 
| twitch    | `string?` | faa 

### Example
```json
{
  "github": "VadyChel",
  "website": "https://vadym.ml",
  "youtube": "someyoutubechannel",
  "discord": "uJJD7Deqyb",
  "twitter": "s1mpleo",
  "vk": "somevk",
  "instagram": "someinstagram",
  "twitch": "sometwitch"
}
```

## Bot Model

| Field         | Type           | Description |
| ------------- | -------------- | ----------- |
| id            | `integer`      | asda |
| user_id       | `snowflake`    | asfasf |
| access_level  | `integer`      | sagfas |
| registered_at | `datetime`     | agfafa |
| status        | `string`       | sfs asf |
| bio           | `string`       | faa 
| bots          | `List[Bot]`    | faa 
| servers       | `List[Server]` | faa 
| social        | `UserSocial`   | faa 
| badges        | `List[string]` | faa 
| verificated   | `boolean`      | faa 
| discord       | `DiscordUser`  | faa 

### Example
```json
{
  "id": 0,
  "user_id": "660110922865704980",
  "access_level": 4,
  "registered_at": "2021-01-01T20:20:00.000000",
  "status": "This is a status",
  "bio": "This is a bio",
  "badges": [],
  "verificated": true,
  "discord": {},
  "servers": [],
  "bots": [],
  "social": {
      "github": "VadyChel",
      "website": "https://vadym.ml",
      "youtube": "someyoutubechannel",
      "discord": "uJJD7Deqyb",
      "twitter": "s1mpleo",
      "vk": "somevk",
      "instagram": "someinstagram",
      "twitch": "sometwitch"
    }
}
```

## Webhook Model

| Field   | Type              | Description |
| --------| ----------------- | ----------- |
| id      | `integer`         | asda |
| user_id | `snowflake`       | asfasf |
| trigger | `string`          | sagfas |
| type    | `string`          | agfafa |
| targets | `List[snowflake]` | sfs asf |
| token   | `string`          | faa 
| url     | `string`          | faa 

### Example
```json
{
  "id": 0,
  "user_id": "660110922865704980",
  "trigger": "bump",
  "type": "bot",
  "targets": ["813065963003052073"],
  "token": "somemegasecuretoken",
  "url": "https://example.com/webhook"
}
```
