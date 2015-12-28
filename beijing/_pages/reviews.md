---
layout: page
title: "影评书评"
permalink: /beijing/reviews/
description: "网友影评书评"
header-img: img/beijing-beihai-park.jpg
---


<h3 class="section-heading text-center">影评</a></h3>
<div class="tiles">
{% for post in site.categories.beijing %}{% if post.categories contains "movies" %}
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <div class="title-desc">{{ post.description }}</div>
{% endif %}{% endfor %}
</div><!-- /.tiles -->

<h3 class="section-heading text-center">书评</a></h3>
<div class="tiles">
{% for post in site.categories.beijing %}{% if post.categories contains "books" %}
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <div class="title-desc">{{ post.description }}</div>
{% endif %}{% endfor %}
</div><!-- /.tiles -->

