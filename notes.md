---
layout: page
title: Note
description: Collective of Notes.
keywords: blog, archive, notes
---
<ul>
	{% for post in site.posts %}
	<a> href="{{post.url}}">{{post.title}}</a>
	{% endfor %}
</ul>