---
description: Add reactions to the message the bot has send in the command.
---

# $addReactions

### Usage

```php
$addReactions[emojis]
```

This function has one field.

1. `emojis` - The emojis to react with, separate emojis using `;`.

### Example

Singular Reaction:

```javascript
bot.command({
    name: "react",
    code: `
    $addReactions[🌸]
    Hi, take a flower
    `
});
```

Multiple Reactions:

```javascript
bot.command({
    name: "question",
    code: `
    $addReactions[✔;❌]
    Does someone reads this?
    `
});
```

