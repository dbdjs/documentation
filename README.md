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

```javascript
const dbd = require("dbd.js");
const bot = new dbd.Bot({
 intents: true,
 prefix: "PREFIX", 
 revertReading: false, 
 })
 
 bot.login("TOKEN")
```

> You must enter a prefix via `PREFIX`

> You must enter a valid Discord Bot Token via `TOKEN`



