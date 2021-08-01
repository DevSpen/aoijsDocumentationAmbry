---
description: Removes links from the provided text.
---

# $removeLinks

### Usage

```php
$removeLink[text]
```

This function has one field.

1. `text` - The text to remove links from. \| Required

### Example

```javascript
bot.command({
name: "example",
code: `$removeNewLines[https://google.com Hello!]`
})
// returns "Hello!"
```

