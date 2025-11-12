---
title: publishing
layout: rest
description: A journey to follow the path of the light
type: parent
order: 2
---

<div class="section main">
	<div class="container">
		{% assign mypages = site.pages | where: "type", "travel" %}
		{% for page in mypages %}
		<a class="button" href="{{ page.url | relative_url }}">{{ page.title }}</a>
		{% endfor %}
	</div>
</div>
