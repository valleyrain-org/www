---
layout: page
title: "分享笔记"
permalink: /note/
description: "每期分享笔记"
---


<h3 class="section-heading text-center">过往笔记</a></h3>
<div class="tiles">
{% for post in site.categories.note %} 
                <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
                <div class="title-desc">{{ post.description }}</div>
{% endfor %}
</div><!-- /.tiles -->

