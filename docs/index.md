---
layout : default
slug: /index
order : 1
---

{%- assign pages = site.pages | sort: "order"  -%}
 
{% for page in pages %}
{{ page.content }}
{% endfor %}  