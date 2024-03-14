---
layout: presentation
---

{% assign pages = site.pages | sort: "order" %}
{% for page in pages %}
 {% if page.utilisation == "global" %}
    {{- page.content | markdownify -}}
  {% endif %}
{% endfor %}