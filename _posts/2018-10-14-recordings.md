---
layout: recordings
title: "Recordings/Reviews"
author: "Zack Browning"
categories: documentation
tags: [recordings]
image: records.jpg
---

# Click on pictures to purchase CD

<p>
{% for item in site.data.recordings %}
    <br>
    <article>
    <a href="{{ item.url }}">
        {% if item.image %}
            <div class="recordings-image">
                <img src="{{ site.github.url }}/assets/img/{{ item.image }}">
            </div>
        {% endif %}
    </a>
        </article> 
            {% if item.listen %}
                <p><h2><a href="{{ item.listen }}"> Listen to {{ item.title }}  ({{item.publisher}}, {{item.year}}) </a></h2></p>
            {% endif %} 

            {% if item.overview %}
                <p>{{item.overview}}</p>
            {% endif %} 

            {% if item.list %}
                <p>
                    <h3>Play List:</h3>
                    <ol>
                        {% for titl in item.list %}
                            <li>
                                <i>{{titl.name}}</i> for {{titl.instrument}} ({{titl.duration}})
                            </li>
                        {% endfor %}
                    </ol>
                </p> 
            {% endif %} 

        {% if item.reviews %}
            <p><h3>Reviews:</h3><ul>
            {% for titl in item.reviews %}
                <li>{{titl.content}}<br><b>-- 
                    {% if titl.author %}{{titl.author}}, {% endif %}
                    {% if titl.review %}"{{titl.review}}." {% endif %}
                    {% if titl.source %}{{titl.source}}, {% endif %}
                    {{titl.issue}}.</b></li>
            {% endfor %}
        </ul></p> 
        {% endif %}

{% endfor %}
</p>
