---
layout: page
permalink: /events/past/
title: "活动回顾"
description: "过往活动回顾"
---

<h3 class="section-heading text-center">往期活动回顾</a></h3>
<div class="tiles">
{% for post in site.categories.event %}
     {% capture nowunix %}{{'now' | date: '%j'}}{% endcapture %}
     {% capture posttime %}{{post.date | date: '%j'}}{% endcapture %}


     {% capture nowyear %}{{'now' | date: '%Y'}}{% endcapture %}
     {% capture postyear %}{{post.date | date: '%Y'}}{% endcapture %}

     {% if postyear > nowyear %} 
  	{% capture posttime %}{{ posttime | plus:'365'}}{% endcapture %}
     {% endif %}

     {% if posttime < nowunix %}
            <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
            <div class="title-desc"><h3>{{post.date | date:"%B %d, %Y" }}</h3></div>
            <div class="title-desc">{{ post.description }}</div>
     {% endif %}
{% endfor %}
</div><!-- /.tiles -->

<h3 class="section-heading text-center">过往笔记</a></h3>
<div class="tiles">
{% for post in site.categories.notes %} 
                <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
                <div class="title-desc">{{ post.description }}</div>
{% endfor %}

