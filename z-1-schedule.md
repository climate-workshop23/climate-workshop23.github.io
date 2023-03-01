---
title: Schedule
nav: true
---

## Workshop Schedule

### **Day 1**

<table>
  <tr><th>Time</th></tr>
  {% for row in site.data.schedule1 %}
  <tr>
    <td>{{ row.time }}</td>
    <td>{{ row.title }}</td>
    <td>{% if row.speaker %}{{ row.speaker }}: {{ row.detail }}{% endif %}</td>
  </tr>
  {% endfor %}
</table>

### **Day 2**

<table>
  <tr><th>Time</th></tr>
  {% for row in site.data.schedule2 %}
  <tr>
    <td>{{ row.time }}</td>
    <td>{{ row.title }}</td>
    <td>{% if row.speaker %}{{ row.speaker }}: {{ row.detail }}{% endif %}</td>
  </tr>
  {% endfor %}
</table>
