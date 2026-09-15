---
layout: default
title: Home
---

# Projects
![alt text hello there](/assets/images/testimage.jpg)
{% assign sorted_projects = site.projects | sort: 'date' | reverse %}
{% for project in sorted_projects %}
### [{{ project.title }}]({{ project.url | relative_url }})
{% include skill-tags.html skills=project.skills %}

{% endfor %}

[Browse everything by skill instead →]({{ '/skills/' | relative_url }})
