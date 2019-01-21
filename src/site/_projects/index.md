---
title: Projects
subtitle: 
tags: 
layout: layouts/base.njk
---

<ul class="listing projects">
{%- for page in collections.project -%}
  <li>
    <a href="{{ page.url }}"><h3>{{ page.data.title }} &rarr;</h3></a>
  </li>
{%- endfor -%}
</ul>