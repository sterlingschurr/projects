---
layout: default
title: Home
---

# Sterling's Projects

(This site is still under construction, so there are still a few missing sections. Feel free to email me if there's one you'd like updated.)

Thanks for coming to view my projects! Below is a list of them all sorted from newest to oldest. There's also a link to sort by skill instead.

![alt text hello there](/assets/images/testimage.jpg)

### AI Policy
Amount and depth of AI usage will always be disclosed on project pages. AI is **never** used for any descriptive text (titles, comments, body text, etc.). Structuring this page to work with Jekyll and CSS formatting was assisted by AI.

# Projects Sorted by Date
[Browse everything by skill instead →]({{ '/skills/' | relative_url }})

{% assign sorted_projects = site.projects | sort: 'date' | reverse %}
{% for project in sorted_projects %}
### [{{ project.title }}]({{ project.url | relative_url }})
{% include skill-tags.html skills=project.skills %}

{% endfor %}


