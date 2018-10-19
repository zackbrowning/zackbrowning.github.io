---
layout: post
title: "Zack Browning Composition"
author: "Zack Browning"
categories: composition
tags: [documentation,sample]
image: zack-2.jpg
---

{% for item in site.data.composition %} <p> <dl> {{item.year}} -- {{item.title}} ({{item.duration}}) </dl> </p> {% endfor %}
