---
title: Speakers
nav: true
---

## Keynote Speakers

{% for speaker in site.data.keynotespeakers %}
### **{{ speaker.name }}**

<div style="content: ''; clear: both; display: table;"><!-- "clearfix hack" so image does not overflow outside container -->
{% include figure.html img=speaker.photo alt=speaker.name style="float:left; margin-right:10px; margin-bottom:10px;" width="40%" %}

{{ speaker.bio }}
</div>
{% endfor %}
