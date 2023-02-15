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

Welcome to the Spring 2023 iteration of Codebreaking At Cal! This course is designed as an upper-division introduction to the field 
of cryptography, which is the science of secure communication (secret messages, encryption, digital signatures, and much more). 

Lectures are once weekly on Monday 6:30 - 8 PM in Soda 306. [Zoom link](https://berkeley.zoom.us/j/94249910215)

**Assignment Extension Request Form**: [https://bit.ly/codebreaking-extension](https://bit.ly/codebreaking-extension)

{% assign newmodules = site.modules | where: 'semester', 'spring' %}
{% for module in newmodules %}
{{ module }}
{% endfor %}

