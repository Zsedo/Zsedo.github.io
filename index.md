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
{% include milestone.md trenutniDenar=trenutniDenar milestone=500 miza="Miza 1" %}
{% include milestone.md trenutniDenar=trenutniDenar milestone=1000 miza="Miza 2" %}
{% include milestone.md trenutniDenar=trenutniDenar milestone=2000 miza="Miza 3" %}

[Donacije](../donacije)
