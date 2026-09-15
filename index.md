---
layout: default
title: Home
---

# Projects

{% assign sorted_projects = site.projects | sort: 'date' | reverse %}
{% for project in sorted_projects %}
### [{{ project.title }}]({{ project.url | relative_url }})
{{ project.skills | join: ", " }}

{% endfor %}

[Browse everything by skill instead →]({{ '/skills/' | relative_url }})
