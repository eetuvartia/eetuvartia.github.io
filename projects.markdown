---
layout: default
title: Projects
permalink: /projects
---
{% assign sorted_projects = site.projects | sort:"order" %}
{% for project in sorted_projects reversed %}
{% if project.display %}
{% include projects/project.html %}
{% endif %}
{% endfor %}