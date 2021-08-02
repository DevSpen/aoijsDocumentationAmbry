---
description: >-
  A command property that you can paste in the command's name field, to trigger
  the command on every message.
---

# $alwaysExecute

This function will allow the command to be executed by every message a user sends.

{% hint style="danger" %}
Use this function wisely.
{% endhint %}

### Usage

```javascript
bot.command({
name: "$alwaysExecute", //$alwaysExecute goes in the command name.
code: `your code here` //Code that will be execute on every message.
})
```

### Example

_This example is a message counter._

```javascript
bot.variables({
messages: 0 //Making the variable
})

bot.command({
name: "$alwaysExecute", 
code: `$setVar[messages;$sum[$getVar[messages];1]]` //Adds 1 to the value for every message sent
})
```

{% hint style="warning" %}
Having alot of `$alwaysExecute` commands  can lead to high ping and delayed responses.
{% endhint %}

