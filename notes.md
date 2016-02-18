---
layout: page
title: Notes
cover: cover.jpg
description: Collective of Notes.
keywords: blog, archive, notes
---

<div class="posts notes">
  {% for post in site.posts %}
    <div class="post-list">
      <div align="right" class="post-list-date">{{ post.date | date: "%b %d, %Y" }}</div>
	    <div align="left" class="text-truncate"><a href="{{ post.url }}">{{ post.title }}</a></div>
      <div align="left" class="post-list-desc"><small>{{ post.description }}</small></div>
    </div>
  {% endfor %}
</div>