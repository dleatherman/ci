---
title: Studio
subtitle: Tuesdays + Fridays 9-11:40AM
layout: layouts/base.njk
---

### Reading

### Lectures

<ul class="listing">
{%- for page in collections.lecture -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay }}</time>
  </li>
{%- endfor -%}
</ul>