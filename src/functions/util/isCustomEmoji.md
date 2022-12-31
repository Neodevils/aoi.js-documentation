---
title: $isCustomEmoji 
description: $isCustomEmoji will check if the given emoji is a custom emoji or not.
id: isCustomEmoji
---

`$isCustomEmoji` will check if the given emoji is a custom emoji or not.

## Usage

```php
$isCustomEmoji[emoji;guildID?]
```

## Parameters 


| Field     | Type    | Description                                        | Required |
|-----------|---------|----------------------------------------------------|----------|
| emoji      | string  | emoji you want to check if it is a custom emoji                           | yes      |
| guildID?     | integer  | guild ID of where the emoji was created in          | no       |

### Please note that your bot has to be in the server where the custom emoji is present in, in order for the function to work properly.

## Example

This will return `true` as the <img src="https://cdn.discordapp.com/emojis/1003365344724910191.webp?size=96&quality=lossless" width="19"> emoji exists:

```javascript
bot.command({
  name: 'isCustomEmoji',
  code: `
  $isCustomEmoji[<:LerefMoney:1003365344724910191>;773352845738115102]
  `
});
```