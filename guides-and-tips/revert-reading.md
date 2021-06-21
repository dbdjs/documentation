---
description: Revert the reading of how functions / codes are function
---

# Revert Reading

## What does _"Revert Reading"_ do?

Revert reading is self explanatory, essentially reverts how codes are able to read from. 

## How do I begin or use it?

It's a very simple process, to begin with you must head over where you define the package.

Then you must add the following `revertReading` below the options.

![Example of adding revertReading](../.gitbook/assets/54b328fcb579639e91fe8e1760a691b7.gif)

## Setup 

{% tabs %}
{% tab title="index.js" %}
```javascript
const dbd = require("dbd.js")

const bot = new dbd.Bot({
  prefix: "!", //Prefix is able to be changed
  revertReading: true, //true or false
})
```
{% endtab %}
{% endtabs %}

## Usage

{% tabs %}
{% tab title="index.js" %}
```javascript
bot.assignType(bot.Types.Message, bot.createCommmand({
  name:"ram", //Command Name
  code:"$pingms - $botPingms" //Code
}))
```
{% endtab %}
{% endtabs %}

{% hint style="info" %}
Once enabled revertReading the functions will be read from bottom to top
{% endhint %}

> The functions are read from top to bottom by default.

> By revert Reading it will read from bottom to top.

