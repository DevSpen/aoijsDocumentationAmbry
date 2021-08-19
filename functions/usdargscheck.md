---
description: >-
  This function will check if the condition is met between the desired number of
  arguments (aka words) and the number of arguments that are actually in the
  user's message.
---

# $argsCheck

### Usage

```php
$argsCheck[number;errorMessage]
```

This function has two fields.

1. `howMany` - How many arguments there should be in the user’s message.

> For example, if you want users to have 3 or more arguments in their message; you can use `>3`. If you want users to have less than 3 arguments in their message, you can use `<3`. If you want the users to have exactly 3 arguments in their message put `3`.

   2. `errorMessage` - The message that the bot will send if the user has too many/little arguments.

### Examples

```javascript
bot.command({
    name: "args",
    code: `
    You have more than two arguments, nice!
    $argsCheck[>2;You have less than two arguments!]
    `
});

//or

bot.command({
    name: "args",
    code: `
    You have two arguments, nice!
    $argsCheck[2;You don't have exactly 2 arguments]
    `
});

//or

bot.command({
    name: "args",
    code: `
    You have less than two arguments, nice!
    $argsCheck[<2;You have more than two arguments!]
    `
});
```

