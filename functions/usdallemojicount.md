---
description: >-
  Returns the total amount of emojis from all the servers the bot is in.
  Optionally, you can filter what type of emojis are included in the count.
---

# $allEmojiCount

### Usage

```php
$allEmojiCount[type (optional)]
```

This function has one field.

1. `type` - The emoji type to return the count for, `all` by default. \| Optional

#### Types

* `all` or empty field - Returns the total amount of custom emojis the bot has access to \(animated and static\).
* `animated` - Returns the total amount of animated custom emojis.
* `normal` - Returns amount of static/regular custom emojis.

### Examples

Total emoji count:

```javascript
bot.command({
name: "emojiCount",
code: `$allEmojiCount emojis`
})
```

Total animated emojis:

```javascript
bot.command({
name: "emojiCount",
code: `$allEmojiCount[animated] emojis`
})
```

Normal emojis:

```javascript
bot.command({
name: "emojiCount",
code: `$allEmojiCount[normal] emojis`
})
```

