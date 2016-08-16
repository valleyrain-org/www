---
layout: page
title: "影评"
permalink: /movies/
description: "书友影评"
---


<h3 class="section-heading text-center">影评</h3>
<div class="tiles">
{% for post in site.categories.movies %}
                <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
                <div class="title-desc">{{ post.description }}</div>
{% endfor %}
</div><!-- /.tiles -->

