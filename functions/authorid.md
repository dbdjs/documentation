---
description: Returns the Author ID of Message
---

# $authorID

## ⚙ Function Usage

```javascript
$authorID
```

## 💻 Function Example

{% tabs %}
{% tab title="index.js" %}
```javascript
bot.assignType(bot.Types.Message, bot.createCommmand({
  name:"authorID",
  code:`Your author ID: $authorID`
}))
```
{% endtab %}
{% endtabs %}

