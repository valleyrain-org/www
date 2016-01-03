---
layout: page
permalink: /events/upcoming/
title: "活动预告 - 旧金山湾区硅谷华人读书会"
description: "近期活动预告"
---

<div class="tiles">
{% for post in site.categories.event reversed %} 
        {% capture nowunix %}{{'now' | date: '%j'}}{% endcapture %}
        {% capture posttime %}{{post.date | date: '%j'}}{% endcapture %}

        {% capture nowyear %}{{'now' | date: '%Y'}}{% endcapture %}
        {% capture postyear %}{{post.date | date: '%Y'}}{% endcapture %}

        {% if postyear > nowyear %} 
  	   {% capture posttime %}{{ posttime | plus:'365'}}{% endcapture %}
        {% endif %}

        {% if postyear < nowyear %} 
           {% capture posttime %}{{ posttime | minus:'365'}}{% endcapture %}
        {% endif %}

        {% if posttime >= nowunix %}
                <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
                <div class="title-desc"><h3>{{post.date | date:"%B %d, %Y" }}</h3></div>
                <div class="title-desc">{{ post.description }}</div>
        {% endif %}
{% endfor %}
</div><!-- /.tiles -->
