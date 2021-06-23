---
description: Return the Package version (current installed)
---

# $packageVersion

## ⚙ Function Usage

```javascript
$packageVersion
```

## 💻 Function Example

{% tabs %}
{% tab title="index.js" %}
```javascript
bot.assignType(bot.Types.Message, bot.createCommmand({
  name:"package-version",
  code:`The current version installed: $packageVersion`
}))
```
{% endtab %}
{% endtabs %}

