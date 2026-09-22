---
layout: default
title: Browse by Skill
permalink: /skills/
---

# Projects Sorted by Skill
![Sort instead by Name](/index.md)

{% assign all_skills = "" | split: "" %}
{% for project in site.projects %}
  {% for skill in project.skills %}
    {% unless all_skills contains skill %}
      {% assign all_skills = all_skills | push: skill %}
    {% endunless %}
  {% endfor %}
{% endfor %}
{% assign all_skills = all_skills | sort %}

<nav class="skill-nav">
{% for skill in all_skills %}<a href="#{{ skill | slugify }}">{{ skill }}</a> {% endfor %}
</nav>

{% for skill in all_skills %}
<h2 id="{{ skill | slugify }}">{{ skill }}</h2>
<ul>
{% assign matching = site.projects | where_exp: "project", "project.skills contains skill" %}
{% for project in matching %}
  <li><a href="{{ project.url | relative_url }}">{{ project.title }}</a></li>
{% endfor %}
</ul>
{% endfor %}
