---
layout: default
---

<div id="home">
  <h1>Stories</h1>
  <ul class="stories">
    {% for story in site.data.stories %}
      <li><span>{{ story.date | date_to_string }}</span> &raquo; <a href="https://www.theguardian.com{{ story.link }}">{{ story.title }}</a></li>
    {% endfor %}
  </ul>
</div>