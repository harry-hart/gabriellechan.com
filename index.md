---
layout: default
---

<div id="home">
  <h1>Blog Posts</h1>
  <ul class="stories">
    {% for story in site.data.stories %}
      <li><span>{{ story.date | date_to_string }}</span> &raquo; <a href="{{ story.link }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>