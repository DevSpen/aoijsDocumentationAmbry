---
description: Return's the given user's activities.
---

# $activity

This function shows the current activity of the indicated user \(Only if it detects any activity.\), If the indicated user does not have an activity such as a 'custom status' it will show 'none'.U

### Usage

```php
$activity[(optional) userID]
```

This function has 1 field.

1. `userID` -  The user the activity is based on. \| Optional

### Activities

* Custom Status
* Spotify _\(Listening to\)_
* &lt;Game Name&gt; _\(Playing\)_
* Streaming

### Examples

Without a userID:

```javascript
bot.command({
    name: "activiy",
    code: `$activity`
});
```

With a userID:

```javascript
bot.command({
    name: "activity",
    code: `$activity[535566311942651924]`
});
```

