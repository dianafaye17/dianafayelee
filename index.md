---
layout: default
title: Diana Lee's Blog
description: Diana Lee's Blog
keywords: blog software web dev 
---

<h2>Recent Posts</h2>

<div class="row">
	<div class="small-12 columns">
		
	{% for post in site.posts limit:1 %}
	<article>
    <a href="{{ post.url }}">
    <h3 class="text-left">{{ post.title }}</h3>
    <br>
    <p class="blogdate">{{ post.date | date: "%d %B %Y" }}</p>
    <div>{{ post.content }}</div>
    </a>
	</article>

	{% endfor %}

	</div>
</div>
