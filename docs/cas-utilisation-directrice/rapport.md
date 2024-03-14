---
layout: default
---


{% assign pages = site.pages | sort: "order" %}
{% for page in pages %}
 {% if page.utilisation == "directrice" %}
    {{- page.content | markdownify -}}
  {% endif %}
{% endfor %}