---
description: Aliases allow users to run the same command using different triggers.
---

# Aliases

### Regular Aliases

```javascript
bot.command({
name: "name",
aliases: ['alias1','alias2'], // aliases here
code: `code`
})
```

_Aliases are listed in a_ [_array_](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)_._

### Aliases for Command Handler

```javascript
module.exports = ({
name: "name",
aliases: ['alias1','aliases2'], // aliases here
code: `code`
})
```

