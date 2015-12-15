---
layout: page
title: "影评书评"
permalink: /reviews/
description: "网友影评书评"
---


<h3 class="section-heading text-center">影评</a></h3>
<div class="tiles">
{% for post in site.categories.movies %} 
                <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
                <div class="title-desc">{{ post.description }}</div>
{% endfor %}
</div><!-- /.tiles -->

<h3 class="section-heading text-center">书评</a></h3>
<div class="tiles">
{% for post in site.categories.books %} 
                <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
                <div class="title-desc">{{ post.description }}</div>
{% endfor %}
</div><!-- /.tiles -->

