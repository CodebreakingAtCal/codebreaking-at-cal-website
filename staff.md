---
layout: page
title: Staff
nav_order: 4
description: A listing of all the course staff members.
---
# Staff

We are lucky to be advised by [Peyrin Kao](https://peyrin.github.io/), the lecturer for CS 161 and CS 188.

## Instructors

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign teaching_assistants = site.staffers | where: 'role', 'TA' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}
## Teaching Assistants

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}
