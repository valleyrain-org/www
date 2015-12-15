---
layout: page
title: "网友原创"
permalink: /la/works/
description: "网友原创作品"
---


<h3 class="section-heading text-center">诗歌</a></h3>
<div class="tiles">
{% for post in site.categories.la %}{% if post.categories contains "poems" %}
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <div class="title-desc">{{ post.description }}</div>
{% endif %}{% endfor %}
</div><!-- /.tiles -->

<h3 class="section-heading text-center">散文随笔</a></h3>
<div class="tiles">
{% for post in site.categories.la %}{% if post.categories contains "essay" %}
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <div class="title-desc">{{ post.description }}</div>
{% endif %}{% endfor %}
</div><!-- /.tiles -->


<h3 class="section-heading text-center">小说</a></h3>
<div class="tiles">
{% for post in site.categories.la %}{% if post.categories contains "novels" %}
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <div class="title-desc">{{ post.description }}</div>
{% endif %}{% endfor %}
</div><!-- /.tiles -->

<h3 class="section-heading text-center">摄影作品</h3>
<div class="tiles">
{% for post in site.categories.la %}{% if post.categories contains "photograph" %}
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <div class="title-desc">{{ post.description }}</div>
{% endif %}{% endfor %}
</div><!-- /.tiles -->

