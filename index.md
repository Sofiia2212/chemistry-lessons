---
---

## Уроки

<ul>
{% for file in site.static_files %}
  {% if file.path contains '/lessons/' %}
    <li><a href="{{ file.path }}">{{ file.name }}</a></li>
  {% endif %}
{% endfor %}
</ul>
