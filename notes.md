---
layout: page
title: Notes
description: Collective of Notes.
keywords: blog, archive, notes
---

<div class="posts notes">
  {% for post in site.posts %}
    <div class="post-list">
      <div align="center" class="post-list-date"><small>{{ post.date | date: "%b %d, %Y" }}</small></div>
	    <div align="center" class="text-truncate"><a href="{{ post.url }}">{{ post.title }}</a></div>
      <div align="center" class="post-list-desc">{{ post.description }}</div>
    </div>
  {% endfor %}
</div>