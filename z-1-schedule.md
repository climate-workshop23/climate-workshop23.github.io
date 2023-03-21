---
title: Schedule
nav: true
---

## Workshop Schedule

{% for day in site.data.schedule %}
### **{{ day.day }}**

<table class="styled-table">
    <thead>
        <tr>
            <th>Time</th>
            <th>Session Title</th>
            <th colspan="2">Speaker</th>
        </tr>
    </thead>
    <tbody>
    {% for row in day.events %}
        <tr{% if row.active %} class="active-row"{% endif %}>
            <td>{{ row.start }}</td>
            {% if row.speaker %}
            <td>{{ row.title }}</td>
            <td>{{ row.speaker }}</td>
            <td>{{ row.topic }}</td>
            {% else %}
            <td colspan="3">{{ row.title }}</td>
            {% endif %}
        </tr>
    {% endfor %}
    </tbody>
</table>

{% endfor %}
