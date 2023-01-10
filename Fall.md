---
layout: page
title: Fall 2022 Archive
nav_exclude: false
nav_order: 6
permalink: fa22.html
seo:
  type: Course
  name: Home
---

# Codebreaking at Cal Fall 2022 Archive

This is an archive of the Fall 2022 offering of the course. Note that many of these materials are now changed in the current iteration.

{% assign oldmodules = site.modules | where: 'semester', 'fall' %}
{% for module in oldmodules %}
{{ module }}
{% endfor %}
