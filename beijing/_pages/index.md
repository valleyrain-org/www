---
layout: page
permalink: /beijing/
title: "北京分部活动"
description: "谷雨书苑北京分部活动页面"
---

<div class="tiles">
{% for post in site.categories.beijing %}
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <div class="title-desc"><h3>{{post.date | date:"%B %d, %Y" }}</h3></div>
    <div class="title-desc">{{ post.description }}</div>
{% endfor %}
</div><!-- /.tiles -->
