---
description: The Official DBD.JS Version 4.0.0x Documentation
---

# Introduction

## Setting up 

To begin you must install the package

{% hint style="warning" %}
You must be on NodeJS v14 and above to ensure it will work properly.
{% endhint %}

```
$ npm i dbd.js@dev
```

{% hint style="info" %}
 This should take approximately couple of seconds to install.
{% endhint %}

Once you've installed the package we can initialize the setup.

{% tabs %}
{% tab title="index.js" %}
```javascript
const dbd = require("dbd.js");
const bot = new dbd.Bot({
 intents: true,
 prefix: "PREFIX", 
 revertReading: false, 
 })
 
bot.enableEvent("message"); //Allow to runs Commands
bot.enableEvent("ready"); //Executes when Client is Ready

const id = bot.createCommmand({code:"$log[$username[$clientID] is Ready.]"});
bot.assignType(bot.Types.Ready, id);
 
 
 bot.login("TOKEN")
```
{% endtab %}
{% endtabs %}

> You must enter a prefix via `PREFIX`

> You must enter a valid Discord Bot Token via `TOKEN`

## Usage of Command

{% tabs %}
{% tab title="index.js" %}
```javascript
bot.assignType(bot.Types.Message, bot.createCommmand({
  name:"command",
  code:"code" 
}))
```
{% endtab %}
{% endtabs %}

## Example + Command

{% tabs %}
{% tab title="index.js" %}
```javascript
const dbd = require("dbd.js");
const bot = new dbd.Bot({
 intents: true,
 prefix: "PREFIX", 
 revertReading: false, 
 })
 
bot.enableEvent("message"); //Allow to runs Commands
bot.enableEvent("ready"); //Executes when Client is Ready

const id = bot.createCommmand({code:"$log[$username[$clientID] is Ready.]"});
bot.assignType(bot.Types.Ready, id);

/*COMMAND EXAMPLE BELOW*/
 bot.assignType(bot.Types.Message, bot.createCommmand({
  name:"ping", //Command Name
  code:"Pong! $pingms" //Returns <Websocket Ping> ms
}))
 
 bot.login("TOKEN")
```
{% endtab %}
{% endtabs %}



