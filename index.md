---
---

## Уроки

<ul>
{% for file in site.static_files %}
  {% if file.path contains '/lessons/' %}
    <li><a href="{{ file.path | relative_url }}">{{ file.name }}</a></li>
  {% endif %}
{% endfor %}
</ul>
