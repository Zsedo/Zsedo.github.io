---
layout: default
---
{% asign trenutniDenar = 0 %}
{% for vplacilo in site.data.vplacila %}
{% assign znesek = vplacilo.znesek | convert = "number" %}
{% asign trenutniDenar = znesek | plus: trenutniDenar %}
{% endfor %}

## Billiards!

{{ site.welcome_text }}

## Trenutno zbran denar
{{ trenutniDenar }}

[Donacije](../donacije)
