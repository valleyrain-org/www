---
layout: page
permalink: /la/events/past/
title: "活动回顾"
description: "过往活动回顾"
pos: "2"
---

<div class="tiles">
{% for post in site.categories.la %}{% if post.categories contains "event" %}
    {% capture nowunix %}{{'now' | date: '%j'}}{% endcapture %}
    {% capture posttime %}{{post.date | date: '%j'}}{% endcapture %}

    {% if posttime < nowunix %}
           <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
           <div class="title-desc"><h3>{{post.date | date:"%B %d, %Y" }}</h3></div>
           <div class="title-desc">{{ post.description }}</div>
    {% endif %}
{% endif %}{% endfor %}
</div><!-- /.tiles -->
