---
description: Adds a new field to the embed.
---

# $addField

This function is in charge of adding a new field to the embed, these containing a limit of 1000 characters each and allowing to use 10 fields per embed.

### Usage

```php
$addField[title;description;inline (optional) (yes/no)]
```

This function has two fields.

1. `name` - The name of the field. \| Required
2. `value` - The value of the field. \| Required
3. `inline` - If 'yes', fields will appear in same line. However, if you have more than 3 fields \(or the fields are just too long\) with inline enabled, the bot will return rows with 3 fields \(2 if there is a thumbnail\) in each row. 'no' by default. \| Optional

### Example

Without inline:

```javascript
bot.command({
    name: "embed",
    code: `$addField[This is an example field name;And this is the field value!]`
});
```

With inline:

```javascript
bot.command({
    name: "embed",
    code: `
    $addField[Inline #;3;yes]
    $addField[Inline #;2;yes]
    $addField[Inline #;1;yes]
    `
});
```

