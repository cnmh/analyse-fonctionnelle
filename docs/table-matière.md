

{%- assign pages = site.pages | sort: "order"  -%}
 
{% for page in pages %}
- [{{ page.name }}]({{site.baseurl}}/{{ page.url }})
{% endfor %}  