---
description: How to setup a Bot Status
---

# Bot Status

### Basic Status

{% hint style="danger" %}
You need to enter the following, in your main file.
{% endhint %}

```javascript
bot.status({
  text: "Text", // Status details.
  type: "PLAYING", // The precense type.
  status: "idle", // The bot's status.
  time: 12 //How often to change between different statuses in seconds (should be 12 or more).
})
```

### Multiple Statuses

```javascript
bot.status({
  text: "text1",
  type: "PLAYING",
  time: 12
})

bot.status({
  text: "text2",
  type: "WATCHING",
  time: 12
})
```

### Types/Statuses

#### Presence Types:

* PLAYING
* WATCHING
* LISTENING
* STREAMING
* COMPETING

#### Status Types:

* online
* dnd
* idle
* invisible

### Streaming Statuses

{% hint style="info" %}
Streaming-Status supports YouTube Video or Twitch Channel URLs.

If you want to enter an URL, use the following:
{% endhint %}

```javascript
bot.status({
text: "Text", 
type: "STREAMING", 
url: "streamLink"
})
```

### Mobile Status

```javascript
const bot = new Aoijs.Bot({
token: "TOKEN", 
prefix: "!",
mobile: true //enables mobile status
})
```

![Example](../../.gitbook/assets/image%20%2862%29.png)

