---
description: >-
  Returns the count of all the channels of the guilds your bot is in. You can
  optionally input types of channels to count.
---

# $allChannelsCount

### Usage

```php
$allChannelsCount[types (optional)]
```

This function has one field.

1. `type` - The channel type\(s\) to include in this count, separate types using `;`. Valid types: text, voice, category, news. \| Optional

### Example

```javascript
bot.command({
name: "channelCount",
code: `
- $allChannelsCount Channels
- $allChannelsCount[category] Categories
- $allChannelsCount[text] Text Channels
- $allChannelsCount[voice] Voice Channels
- $allChannelsCount[news] Announcement Channels
`
})
```

