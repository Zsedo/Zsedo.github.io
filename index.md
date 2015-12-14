---
layout: default
---
{% asign trenutniDenar = 0 %}
{% for vplacilo in site.data.vplacila %}
{% assign trenutniDenar = trenutniDenar + vplacilo.znesek %}
{% endfor %}

## Billiards!

{{ site.welcome_text }}

## Trenutno zbran denar
{{ trenutniDenar }}

## Milestones:

| Completed | Znesek | Miza |
| :---: | :---: | :---: |
| a | b | c |

[Donacije](../donacije)
