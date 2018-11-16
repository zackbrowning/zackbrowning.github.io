---
layout: default
title: "Composition"
author: "Zack Browning"
categories: documentation
tags: [composition]
image: zack-2.jpg
---

{% for post in site.categories.composition %}<article><a href="{{ site.github.url }}{{ post.url }}"><div class="featured-posts" {% if post.image %}style="background-image:url({{ site.github.url }}/assets/img/{{ post.image }})"{% endif %}><h2><span>{{ post.title }}</span></h2></div></a></article>{% endfor %}


<article>
	<a href="https://www.ideals.illinois.edu/handle/2142/24031">
		<div class="featured-posts" style="background-image:url({{ site.github.url }}/assets/img/zb3.jpg)">
			<h2><span>Kim, Sunjin. Zack Browning and the Compositional Process in Blockhouse, Double Shot, and Sole Injection.</span></h2>
		</div>
	</a>
</article>
