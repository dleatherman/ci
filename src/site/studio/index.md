---
title: Studio
subtitle: Tuesdays + Fridays 9-11:40AM
layout: layouts/base.njk
---

## [Projects](/projects)

### Agendas

<ul class="listing">
{%- for page in collections.agendas | reverse -%}
  <li>
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay }}</time><br>
    <a href="{{ page.url }}">{{ page.data.title }}</a>
  </li>
{%- endfor -%}
</ul>