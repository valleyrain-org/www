---
layout: page
title: "谷雨动态"
permalink: /news/
description: "有关于谷雨书苑的新闻动态"
---


<h3 class="section-heading text-center">谷雨新闻</a></h3>
<div class="tiles">
{% for post in site.categories.news %} 
                <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
                <div class="title-desc">{{ post.description }}</div>
{% endfor %}
</div><!-- /.tiles -->

