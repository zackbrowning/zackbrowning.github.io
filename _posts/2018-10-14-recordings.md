---
layout: default
title: "Recordings"
author: "Zack Browning"
categories: documentation
tags: [recordings]
image: city-1.jpg
---

{% for item in site.data.recordings %}<article><a href="{{ item.url }}"><div class="featured-posts" {% if item.image %}style="background-image:url({{ site.github.url }}/assets/img/{{ item.image }})"{% endif %}><h2><span>{{ item.title }}</span></h2></div></a></article> <p><h3>Play List:</h3><ol>{% for titl in item.list %}<li>{{titl.name}}</li>{% endfor %}</ol></p> <p><h3>Review:</h3><ol>{% for titl in item.reviews %}<li>{{titl.source}}</li>{% endfor %}</ol></p>{% endfor %}
