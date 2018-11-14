---
layout: post
title: "Zack Browning Composition List"
author: "Zack Browning"
categories: composition
tags: [documentation,sample]
image: zack-2.jpg
---

{% for item in site.data.composition %} <p> <dl> {{item.year}} -- <b>{{item.title}}</b> for {{item.instrument}}. ({{item.duration}})  [(audio)]({{item.audio}})  [(video)]({{item.video}}) {% endfor %}
