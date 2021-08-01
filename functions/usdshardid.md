---
description: Returns the current shard ID for the server that this command was ran in.
---

# $shardID

{% hint style="info" %}
View the sharding guide [here](https://aoi.leref.ga/guide/extras/sharding)!
{% endhint %}

## Example

```javascript
bot.command({
name: "shard",
code: `This server is on shard $shardID.`
})
```

