---
layout: page
title: Writing
permalink: /blog/
---
Notes and occasional writing on algorithms, optimisation, computer science and other things I find interesting.

{% if site.posts.size > 0 %}
<div class="post-list">
{% for post in site.posts %}
  <a class="post-item" href="{{ post.url | relative_url }}"><span class="post-date">{{ post.date | date: "%b %Y" }}</span><span class="post-title">{{ post.title }}</span><span class="post-arrow">↗</span></a>
{% endfor %}
</div>
{% else %}
<p class="empty-state">No posts yet. This section is ready for the first one.</p>
{% endif %}