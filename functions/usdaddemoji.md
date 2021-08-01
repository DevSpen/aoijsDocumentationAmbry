---
description: Adds an emoji to the guild.
---

# $addEmoji

###  Usage

```php
$addEmoji[imageURL;emojiName;returnEmoji (yes/no) (optional);roleIDs (optional)]
```

{% hint style="info" %}
The imageURL must be under 256kb in size.
{% endhint %}

This function has four fields.

1. `imageURL` - The URL of the image/gif that's being converted to an emoji. \| Required
2. `emojiName` - The name of the emoji. \| Required
3. `returnEmoji (yes/no)` - Whether to return the emoji that was newly created. \| Optional
4. `roleIDs` - List of role IDs they should have access to this emoji. Only members with these role would have access to see and use that emoji. Leave it empty to set to everyone, separate roleIDs using `;`. \| Optional

### Example

```javascript
bot.command({
    name: "add-emoji",
    code: `$addEmoji[https://cdn.discordapp.com/emojis/786763619438166036.png;shy_bear;yes]`
});
```

![](../.gitbook/assets/mtt45fdb8q.png)

{% hint style="warning" %}
The imageURL needs to end in `.gif`, `.png`, or `.jpg.`
{% endhint %}

