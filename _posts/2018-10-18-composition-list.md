---
layout: post
title: "Zack Browning Composition List"
author: "Zack Browning"
categories: composition
tags: [documentation,sample]
image: zack-2.jpg
---

{% for item in site.data.composition %} <p> <dl> {{item.year}} -- <u>{{item.title}}</u> for {{item.instrument}}. ({{item.duration}}) </dl> </p> {% endfor %}
