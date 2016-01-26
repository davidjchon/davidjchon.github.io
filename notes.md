---
layout: page
title: Notes
description: Collective of Notes.
keywords: blog, archive, notes
---

<div class="post notes">
	{% for post in site.posts %}
		<div class="post-list">
			<div class="post-list-date"><small>{{ post.date | date: "%b %d, %Y" }}</small></div>
				<div class="text-truncate"><a href="{{ post.url }}">{{ post.title }}</a></div>
			<div class="post-list-desc">{{ post.description }}</div>
		</div>
	{% endfor %}
</div>
<div class="posts">
	<ul class="posts-list">
		{% for post in site.posts %}
            <li class="post-link">
                <a class="post-title" href="{{ post.url }}">
                	<span class="post-date">{{ post.date | date_to_string }}</span>
                  	{{ post.title }}
                </a>
            </li>
        {% endfor %}
    </ul>
</div>