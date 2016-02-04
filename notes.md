---
layout: page
title: Notes
description: Collective of Notes.
keywords: blog, archive, notes
---
<!-- <ul>
	{% for post in site.posts %}
	<a> href="{{post.url}}">{{post.title}}</a>
	{% endfor %}
</ul>
 -->
<div class="posts notes">
  {% for post in site.posts %}
    <div class="post-list">
      <div class="post-list-date"><small>{{ post.date | date: "%b %d, %Y" }}</small></div>
	    <div class="text-truncate"><a href="{{ post.url }}">{{ post.title }}</a></div>
      <div class="post-list-desc">{{ post.description }}</div>
    </div>
  {% endfor %}
</div>