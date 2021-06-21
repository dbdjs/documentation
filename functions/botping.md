---
description: Returns the Message Ping
---

# $botPing

## ⚙ Function Usage

```javascript
$botPing
```

## 💻 Function Example

{% tabs %}
{% tab title="index.js" %}
```javascript
bot.assignType(bot.Types.Message, bot.createCommmand({
  name:"message-ping",
  code:`The current Message Ping: $botping`
}))
```
{% endtab %}
{% endtabs %}

