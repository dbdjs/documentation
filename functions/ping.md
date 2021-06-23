---
description: Return the Client Websocket Ping
---

# $ping

## ⚙ Function Usage

```javascript
$ping
```

## 💻 Function Example

{% tabs %}
{% tab title="index.js" %}
```javascript
bot.assignType(bot.Types.Message, bot.createCommmand({
  name:"ping",
  code:`Pong! $pingms (ws)`
}))
```
{% endtab %}
{% endtabs %}

