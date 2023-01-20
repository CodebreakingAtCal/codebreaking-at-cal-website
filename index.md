---
layout: home
nav_order: 0
---

{%- if site.under_construction -%}
<p class="warning">
This site is under construction. All dates and policies are tentative until this message goes away.
</p>
{%- endif -%}

# {{ site.title }}


Welcome to the Spring 2023 iteration of Codebreaking At Cal! This course is designed as an upper-division introduction to the field 
of cryptography, which is the science of secure communication (secret messages, encryption, digital signatures, and much more). 

Lectures are once weekly on Monday 6:30 - 8 PM in Soda 306. [Zoom link](https://berkeley.zoom.us/j/94249910215)

**If you are interested in enrolling for Spring 2023, please fill out this Google form:** [https://forms.gle/6mVieVFGmRuGbpSr9](https://forms.gle/6mVieVFGmRuGbpSr9).

We strictly require **CS 61A** and **CS 70** or their equivalents for this course. CS 161, MATH 113, and CS 170 are helpful, but not required.

## Calendar

[Skip to current week](#week-{{ 'now' | date: '%U' }}){: .btn .btn-outline .fs-3 }

<div>
{%- include syllabus.html -%}
</div>
