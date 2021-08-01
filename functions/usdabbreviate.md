---
description: Abbreviates large numbers.
---

# $abbreviate

### Usage

```php
$abbreviate[number]
```

This function has 1 field.

1. `number` - The number to abbreviate. \| Required

### Abbreviations

* k - thousands
* m - millions
* b - billions
* t - trillions

### Example

```javascript
bot.command({
name: "abbr",
code: `
$abbreviate[5000]
`
//Returns: 5k
})

//or specified number

bot.command({
name: "abbr",
code: `
$abbreviate[$message]
`
})
```

