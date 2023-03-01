---
title: Organisers
nav: true
---

## Organisers

<div style="display: flex; flex-wrap: wrap;">
{% for organiser in site.data.organisers %}
<div style="flex: 0 0 120px; text-align: center;">
{% if organiser.url %}<a href="{{ organiser.url }}">{% endif %}
<img src="images/{{ organiser.photo }}" style="width: 100px; height: 100px; border-radius: 50%;">
<div>
{{ organiser.name }}
</div>
{% if organiser.url %}</a>{% endif %}
</div>
{% endfor %}
</div>
