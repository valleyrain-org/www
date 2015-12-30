---
layout: page
title: "书评- 旧金山湾区硅谷华人读书会"
permalink: /books/
description: "书友书籍推荐及评论"
---

<h3 class="section-heading text-center">书评</a></h3>
<div class="tiles">
{% for post in site.categories.books %} 
                <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
                <div class="title-desc">{{ post.description }}</div>
{% endfor %}
</div><!-- /.tiles -->

