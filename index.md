---
layout: default
---

{% for vplacilo in site.data.vplacila %}
{% if vplacilo.ime == "Skupaj" %}
{% assign trenutniDenar = vplacilo.znesek | convert = "number" %}
{% endif %}
{% endfor %}

## Billiards!

{{ site.welcome_text }}

## Trenutno zbran denar
{{ trenutniDenar }}

## Milestones:

| Completed | Znesek | Miza |
| :---: | :---: | :---: |
{% include milestones.md trenutniDenar=trenutniDenar milestone=500 miza="Miza 1" %}
{% include milestones.md trenutniDenar=trenutniDenar milestone=1000 miza="Miza 2" %}
{% include milestones.md trenutniDenar=trenutniDenar milestone=2000 miza="Miza 3" %}

[Donacije](../donacije)
