[yes]: {{ site.url }}pictures/yes_small.png "Yes"
[no]: {{ site.url }}pictures/no_small.png "No"

{% if trenutniDenar < milestone %}
![][no] | milestone | miza
{% else %}
![][yes] | milestone | miza
{% endif% }