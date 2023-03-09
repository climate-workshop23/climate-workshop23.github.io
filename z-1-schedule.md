---
title: Schedule
nav: true
---

## Workshop Schedule

{% for day in site.data.schedule1 %}
### **{{ day.day }}**

<table class="styled-table">
    <thead>
        <tr>
            <th>Time</th>
            <th>Session Title</th>
            <th>Speaker</th>
        </tr>
    </thead>
    <tbody>
    {% for row in day.events %}
        <tr{% if row.active %} class="active-row"{% endif %}>
            <td>{{ row.start }}</td>
            <td>{{ row.title }}</td>
            <td>{{ row.speaker }}</td>
        </tr>
    {% endfor %}
    </tbody>
</table>

{% endfor %}
