---
layout: page
title: "网友原创"
permalink: /works/
description: "网友原创作品"
---


<h3 class="section-heading text-center">诗歌</a></h3>
<div class="tiles">
{% for post in site.categories.poems %} 
                <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
                <div class="title-desc">{{ post.description }}</div>
{% endfor %}
</div><!-- /.tiles -->

<h3 class="section-heading text-center">散文随笔</a></h3>
<div class="tiles">
{% for post in site.categories.essay %} 
                <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
                <div class="title-desc">{{ post.description }}</div>
{% endfor %}
</div><!-- /.tiles -->


<h3 class="section-heading text-center">小说</a></h3>
<div class="tiles">
{% for post in site.categories.novels %} 
                <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
                <div class="title-desc">{{ post.description }}</div>
{% endfor %}
</div><!-- /.tiles -->

<h3 class="section-heading text-center">摄影作品</h3>
<div class="tiles">
{% for post in site.categories.photograph %} 
                <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
                <div class="title-desc">{{ post.description }}</div>
{% endfor %}
</div><!-- /.tiles -->

