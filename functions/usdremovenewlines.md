---
description: Removes new lines from the provided text.
---

# $removeNewLines

### Usage

```php
$removeNewLines[text]
```

This function has one field.

1. `text` - The text to remove new lines from. \| Required

### Example

```javascript
bot.command({
name: "example",
code: `$removeNewLines[Hello
World]`
})
// returns "Hello World"
```

