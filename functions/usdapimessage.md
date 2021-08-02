---
description: Sends a Message using raw Discord API.
---

# $apiMessage



{% hint style="warning" %}
This function is intended for advanced users of Aoi.JS.
{% endhint %}

### Usage

```php
$apiMessage[content;embed;component;referenceMessageID:mentionTheUser(yes/no);return ID (yes/no)]"
```

This function has 5 fields.

1. `content` - Sends the normal message.
2.  `embed` - Sends the embedded message, uses Embed Errors.
3. `components` - Same as in [interactionReply](usdinteractionreply.md#components).
4. `reference` - This is for replying to the user.

> **Format:** messageID:mentionTheUser\(yes/no\)

    5.  `returnID` - Whether to return the ID of the message sent.

### Example

```javascript
bot.command({
name:"hi",
code:`
$apiMessage[hi;{author:hi::}{title:hello}{field:ok:lol:no}{color:#8700ff}{footer:hmmm:$authorAvatar};;$messageID:true;no]
`
})
```

