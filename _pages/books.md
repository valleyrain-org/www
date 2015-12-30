---
layout: page
title: "书籍影视推荐-谷雨书苑-硅谷读书会"
permalink: /books/
description: "硅谷读书会谷雨书苑为你推荐书籍以及影视作品，附书评和影评"
---

<h3 class="section-heading text-center">书评</a></h3>
<div class="tiles">
{% for post in site.categories.books %} 
                <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
                <div class="title-desc">{{ post.description }}</div>
{% endfor %}
</div><!-- /.tiles -->

