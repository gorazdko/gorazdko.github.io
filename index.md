---
layout: home
title: My Blog
---

# Welcome to My Blog

This is my blog where I share thoughts on tech and more.

## My Blog Posts

{% for post in site.posts %}
  <article>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt }}</p>
    <small>{{ post.date | date: "%B %d, %Y" }}</small>
  </article>
{% endfor %}
