---
description: Returns the author's avatar URL.
---

# $authorAvatar

This function returns the URL of the avatar of the person who ran this command.

### Usage

```php
$authorAvatar
```

### Example

```javascript
bot.command({
    name: "my-avatar",
    code: `$image[$authorAvatar]`
});
```

