---
title: Speakers
nav: true
---

{% for group in site.data.speakers %}
## {{ group.heading }}

{% for speaker in group.speakers %}
<h3><a href="{{ speaker.url }}">{{ speaker.name }}</a></h3>

<div style="content: ''; clear: both; display: table;"><!-- "clearfix hack" so image does not overflow outside container -->
{% include figure.html img=speaker.photo alt=speaker.name style="float:left; margin-right:1ex; margin-bottom:1ex;" width="40%" %}
{{ speaker.bio }}
</div>
{% endfor %}
{% endfor %}
