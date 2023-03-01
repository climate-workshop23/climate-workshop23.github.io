---
title: Organisers
nav: true
---

## Organisers

<div style="display: flex; flex-wrap: wrap;">
{% for organiser in site.data.organisers %}
<div style="flex: 0 0 120px; text-align: center;">
<img src="images/{{ organiser.photo }}" style="width: 100px; height: 100px; border-radius: 50%;">
<div>
{{ organiser.name }}
</div>
</div>
{% endfor %}
</div>
