---
layout: default
---

{% for vplacilo in site.data.vplacila %}
{% if vplacilo.ime == "Skupaj" %}
{% assign trenutniDenar = vplacilo.znesek %}
{% endif %}
{% endfor %}

## Billiards!

{{ site.welcome_text }}

## Trenutno zbran denar
{{ trenutniDenar }}

## Milestones:

| Completed | Znesek | Miza |
| :---: | :---: | :---: |

[Donacije](../donacije)
