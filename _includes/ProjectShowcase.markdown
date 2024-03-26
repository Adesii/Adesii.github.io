{: .text-center }

### Projects

---

{% for years in (2017..2024) reversed %}

# {{years}}

{% assign projects = site.data.projects | where: "year", {{years}} %}
{% include ProjectRow.html %}
{% endfor %}
