---
title: "Home"
layout: textlay
excerpt: "COLAB at EOS-SFSU."
sitemap: false
permalink: /allnews.html
---

<br>

## News

<div style="text-align:justify" markdown="1">

<ul class="posts">

  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></li>
  {% endfor %}

</ul>
