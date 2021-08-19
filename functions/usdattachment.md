---
description: Adds an attachment to the message.
---

# $attachment

This function allows you to add 'attachments' to a message, like images or videos.

### Usage

```php
$attachment[URL]
```

This function has one field.

1. URL - The URL of the attachment. \| Required

### Example

```javascript
bot.command({
    name: "dog",
    code: `$attachment[https://cdn.discordapp.com/attachments/773357374328012840/780585674541105152/20201116_133035.jpg] Take a pic of Kuba's dog!`
});
```

