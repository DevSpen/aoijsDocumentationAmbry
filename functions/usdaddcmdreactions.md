---
description: Adds a reaction to the message that triggered this command.
---

# $addCmdReactions

### Usage

```php
$addCmdReactions[emoji(s)]
```

This function has one field.

1. `emoji(s)` - The emojis to react with, separate emojis using `;`. \| Required

### Examples

```javascript
bot.command({  
    name: "react",
    code: `$addCmdReactions[✔]`
})
```

```javascript
bot.command({
    name: "react",
    code: `$addCmdReactions[🎉;✔]`
});
```

