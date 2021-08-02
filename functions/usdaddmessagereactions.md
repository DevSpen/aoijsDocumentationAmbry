---
description: Adds reaction(s) to the specified message.
---

# $addMessageReactions

### Usage

```php
$addMessageReactions[channelID;messageID;reactions]
```

This function has three fields.

1. `channelID` - The channel of which the 'messageID' is in. \| Required
2. `messageID` - The message to the reactions will get added to. \| Required
3. `reactions` - The emojis of which will be reacted to the message. Separate emojis using `;`. \| Required

### Example

Singular Reaction:

```javascript
bot.command({
    name: "react",
    code: `
    $addMessageReactions[$channelID;$messageID;🌸]
    Here's a pretty flower
    `
});
```

Multiple Reactions:

```javascript
bot.command({
    name: "question",
    code: `
    $addMessageReactions[$channelID;$messageID;✔;❌]
    `
});
```

