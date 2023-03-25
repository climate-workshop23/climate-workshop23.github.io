---
title: Speakers
nav: true
---

{% for group in site.data.keynotespeakers %}
## {{ group.heading }}

{% for speaker in group.speakers %}
### **{{ speaker.name }}**

<div style="content: ''; clear: both; display: table;"><!-- "clearfix hack" so image does not overflow outside container -->
{% include figure.html img=speaker.photo alt=speaker.name style="float:left; margin-right:1ex; margin-bottom:1ex;" width="40%" %}
{{ speaker.bio }}
</div>
{% endfor %}
{% endfor %}
