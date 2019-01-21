---
title: Lab
subtitle: Wednesdays 7-9:40PM
layout: layouts/base.njk
---

<h4>Labs</h4>
<ul class="listing">
{%- for page in collections.lab -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay }}</time>
  </li>
{%- endfor -%}
</ul>



