---
description: Removes special characters from the provided text.
---

# $removeSpecialChars

### Usage

```php
$removeSpecialChars[text]
```

This function has one field.

1. `text` - The text to remove special characters from. \| Required

### Example

```javascript
bot.command({
name: "example",
code: `$removeSpecialChars[Hello World 123! ()*&^%#]`
})
// returns "Hello World 123"
```





