---
layout : default
slug: /index
order : 1
---

 
{%- assign chapitres = site.pages | sort: "order"  -%}
 
{% for chapitre in chapitres %}
- [{{ chapitre.name }}]({{site.baseurl}}/{{ chapitre.url }})
{% endfor %}  
 