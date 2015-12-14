[yes]: {{ site.url }}pictures/yes_small.png "Yes"
[no]: {{ site.url }}pictures/no_small.png "No"

{% if include.trenutniDenar < include.milestone %}
![][no] | include.milestone | include.miza
{% else %}
![][yes] | include.milestone | include.miza
{% endif% }