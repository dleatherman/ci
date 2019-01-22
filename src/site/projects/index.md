---
title: Projects
subtitle: 
tags: 
layout: layouts/base.njk
---

There will be two small projects and three large projects to be completed between studio and lab. Studio will focus on concept, design, presentation, and execution. Lab will focus more in depth on programming. You will receive a grade from both professors. Full descriptions of each project will be posted on this site.

<ol class="listing projects">
{%- for page in collections.project -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }} &rarr;</a>
  </li>
{%- endfor -%}
</ol>