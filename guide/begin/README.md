---
description: The page to guide you with Aoi.JS.
---

# Getting Started

## Installation

{% hint style="warning" %}
**Node.JS 12.0.0 or newer is required.**
{% endhint %}

{% tabs %}
{% tab title="Terminal" %}
```text
npm install aoi.js
```
{% endtab %}
{% endtabs %}

Once this has installed you can begin the following file `index.js` to setup Aoi.JS.

{% tabs %}
{% tab title="index.js" %}
```javascript
const aoijs = require("aoi.js")

const bot = new aoijs.Bot({
token: "TOKEN", //Discord Bot Token
prefix: "PREFIX" //Discord Bot Prefix
})
bot.onMessage() //Allows to execute Commands

bot.command({
name: "ping", //Trigger name (command name)
code: `Pong! $pingms` //Code
})

bot.readyCommand({
    channel: "", //You can use this or not
    code: `$log[Ready on $userTag[$clientID]]` //Example Ready on Client
})
```
{% endtab %}
{% endtabs %}

{% hint style="info" %}
* You must enter a prefix via `PREFIX`
* You must enter a valid Discord Bot Token via `TOKEN`
{% endhint %}

## package.json

{% hint style="warning" %}
For most hosting services, you will need a `package.json` file.
{% endhint %}

If you need a example, there's a quick example to use.

{% tabs %}
{% tab title="package.json" %}
```javascript
{
    "name": "-asdf",
    "version": "1.0.0",
    "description": "",
    "main": "index.js", //replace 'index.js' with your main file name.
    "scripts": {
      "start": "node index.js" //replace 'index.js' with your main file name.
    },
    "engines": {
      "node": "12.x"
    },
    "author": "",
    "license": "ISC",
    "dependencies": {
      "aoi.js": "^4.2.1"
    }
  }
```
{% endtab %}
{% endtabs %}

{% hint style="info" %}
`4.2.1` can be changed to any version number as you want.
{% endhint %}

