---
layout: presentation
order: 1
---

{% assign pages = site.pages | sort: "order" %}
{% for page in pages %}
 {% if page.presentationPackage == "cas-utilisation-médecine-général" %}
    {{- page.content | markdownify -}}
  {% endif %}
{% endfor %}