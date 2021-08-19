---
description: Adds a property (Key) to an existing object.
---

# $addObjectProperty

With this function you can add properties \(keys\) to an object previously created in JSON format.

### Usage

```php
$addObjectProperty[key;value]
```

This function has two fields.

1. Key - The "name" of the object value. \| Required
2. Value - The value that's assigned to the 'key'. \| Required

### Example

```javascript
bot.command({
    name: "add-object-property",
    code: `$getObjectProperty[fact]
    $addObjectProperty[fact;Kuba is cool]
    $createObject[{}]`
});
```

