---
description: Using Aoi.JS Sharding System to allow Sharding for your Client.
---

# Sharding



{% hint style="danger" %}
Sharding is only necessary for bots in 2,000+ Guilds
{% endhint %}

### Enabling Sharding

Just by enable sharding inside of the Client Option, and your Client will be sharding. It's simple and quick!

```javascript
sharding: true,
shardAmount: 2,
```

For example:

```javascript
const bot = new Aoijs.bot({
    sharding: true,
    shardAmount: 2,
    token: "token",
    prefix: "prefix"
})
```

### Finding the Current Guild's Shard

```javascript
bot.command({
    name: "shardID",
    code: `Guilds Shard: $shardID`
})
```

{% hint style="danger" %}
Sharding can lead to high ping/response time and depending your host, it can use a lot of memory and disk space.
{% endhint %}

