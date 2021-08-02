---
description: Allows use of multiple text splits in one message.
---

# $advancedTextSplit

{% hint style="warning" %}
This function is only recommended to use as advanced Aoi.js user because it's hard to understand.
{% endhint %}

### Usage

```php
$advancedTextSplit[text;separator;index;separator2;index2;...]
```

This function has three required fields.

1. `text` - The text to split. \| Required
2. `separator` - The separator of the text which is used for the index. \| Required
3. `index` - The position of the certain text to pull from, 'text' depending the 'separator'. \| Required

_Note: You can repeat fields 2 and 3 multiple times._

### Example

```javascript
bot.command({
name: "advancedtextsplit",
code: `$advancedTextSplt[hi/bye|ok;/;2;|;1]`
})

/*  Code breakdown 
Our first separator is / and we want to return the 2nd index.
the code above returns "bye|ok"
Now the second separator is | and we want to return the 1st index.
so if our text is "bye|ok", then the first index would be "bye"
*/
```

