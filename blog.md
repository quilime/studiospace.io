---
layout: page
title: studiospace blog
background-image: /media/sunset.jpg
---

## Blog

{% for post in site.posts %}
    {% if post.layout != "event" %}
      
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  
  <p class="author">
    <span class="author">{{ post.author }}</span>
    <span class="date">{{ post.date }}</span>
  </p>
  
  <div class="content">
    {{ post.content }}
  </div>
        
  {% endif %}
{% endfor %}
  