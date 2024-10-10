---
title: "Cann | Research"
layout: piclay
excerpt: "Research"
sitemap: false
permalink: /research/
---


## Research topics

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
 <h4 style="font-size:28px"><b><a href="{{ publi.link.url }}"><pubtit>{{ publi.title }}</pubtit></a></b></h4>
 
 <p><b><a href="{{ publi.link.url }}">
 <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="100%" />
 </a></b></p> 

  <p style="text-align:justify; font-size:20px">{{ publi.description }}</p>
  
  <p><em>{{ publi.authors }}</em></p>
  
  <p><b><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></b></p>
  <p class="text-danger"><b> {{ publi.news1 }}</b></p>
  
  <p> {{ publi.news2 }}</p>
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


