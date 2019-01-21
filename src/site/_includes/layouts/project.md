---
layout: layouts/base.njk
pageClass: posts
templateEngineOverride: njk, md
---

<p class="date">
  Assigned: <time datetime="{{ date }}">{{ date | dateDisplay }}</time><br>
  Due: <time datetime="{{ dueDate }}">{{ dueDate | dateDisplay }}</time>
</p>
<main>
  {{ content | safe }}
  <div class="footnote">
  </div>
</main>
