---
layout: home
title: Home
nav_exclude: false
nav_order: 1
permalink: index.html
seo:
  type: Course
  name: Home
---

# Codebreaking at Cal

Welcome to the Fall 2022 iteration of Codebreaking At Cal! This course focuses on cryptography's application to real-world scenarios, and how to break various encryption schemes. 


{% for module in site.modules %}
{{ module }}
{% endfor %}

