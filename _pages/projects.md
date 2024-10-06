---
title: "Projects"
layout: gridlay
excerpt: "Projects"
sitemap: false
permalink: /projects/
---


## Research topics

{% assign number_printed = 0 %}
{% for publi in site.data.projectlist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <p><strong><a href="{{ publi.link.url }}"> <img src="{{ site.url }}{{ site.baseurl }}/images/projectpic/{{ publi.image }}" width="100%" /> </a></strong></p>
  <p><strong><a href="{{ publi.link.url }}"> <h3><pubtit>{{ publi.title }}</pubtit> </h3></a></strong></p>
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.keywords }}</em></p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>


