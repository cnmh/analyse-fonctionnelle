---
layout: presentation
order: 1
---

{% assign pages = site.pages | sort: "order" %}
{% for page in pages %}
 {% if page.scenario == "scenarioderectrice" %}
    {{- page.content | markdownify -}}
  {% endif %}