---
layout: collection
title: Projects
permalink: /projects/
collection: projects
---

# Projects

Welcome to my projects page! Here you'll find a curated list of my work.

{% for project in site.projects %}
## [{{ project.title }}]({{ project.url | relative_url }})
{{ project.description }}

{% endfor %}