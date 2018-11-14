---
layout: default
title: "Composition"
author: "Zack Browning"
categories: documentation
tags: [recordings]
image: zack-2.jpg
---

{% for item in site.data.recordings %}<article><a href="{{ item.url }}"><div class="featured-posts" {% if post.image %}style="background-image:url({{ site.github.url }}/assets/img/{{ item.image }})"{% endif %}><h2><span>{{ item.title }}</span></h2></div></a></article>{% endfor %}
