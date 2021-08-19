---
description: >-
  This function will make the bot reply when a user reacts with the given button
  to the command.
---

# $awaitButtons

### **Usage**

```php
$awaitButtons[messageID;userFilter;customID,customID,...;awaitcommand,awaitedcommand,...;errorContent,errorEmbed,errorFlags (optional);uses (optional)]
```

This function has 8 fields.

1. `messageID` - The ID of the message on which it expects an action.
2. `userFilter` - Use `everyone` or a userID to filter who can react.
3. `customID` - The custom ID of this button. Separate custom IDs using`,`.`b`uterror - The message when the time runs out
4. * uses - number of uses. default 1

Raw Usage:

## **Options**

* * \*\*\*\*

## **Usage**

```javascript
$awaitButtons[$get[id];$authorID;click;awaitclick; Stop,{description:Only $userTag Can Use This Button}{color:#ff0000},64;1]
$let[id;$apiMessage[Click Me;;{actionRow:Click Me,2,1,click};;yes]]
```

{% hint style="info" %}
This will be easier to do in future updates.
{% endhint %}

