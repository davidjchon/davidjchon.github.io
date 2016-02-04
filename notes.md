---
layout: page
title: Note
description: Collective of Notes.
keywords: blog, archive, notes
---
<ul>
	{% for post in site.posts %}
	<h2>
		<a> href="{{post.url}}">{{post.title}}</a>
	</h2>
	{% endfor %}
</ul>