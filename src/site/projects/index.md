---
title: Projects
subtitle: 
tags: 
layout: layouts/base.njk
---

<ol class="listing projects">
{%- for page in collections.project -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }} &rarr;</a>
  </li>
{%- endfor -%}
</ol>