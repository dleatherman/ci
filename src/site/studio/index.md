---
title: Studio
subtitle: Tuesdays + Fridays 9-11:40AM
layout: layouts/base.njk
---

<ul class="listing">
  <li>
    <a href="https://prmlg.ht/cisp19" target="_blank">Syllabus</a>
  </li>
  <li>
    <a href="/projects/">Projects</a>
  </li>
  <li>
    <a href="/studio/readings/">Readings</a>
  </li>
</ul>

### Agendas

<ul class="listing">
{%- for page in collections.agendas | reverse -%}
  <li>
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay }}</time>: <a href="{{ page.url }}">{{ page.data.title }}</a>
  </li>
{%- endfor -%}
</ul>