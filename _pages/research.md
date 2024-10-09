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
 <p><strong><a href="{{ publi.link.url }}"><pubtit><h4>{{ publi.title }}</h4></pubtit></a></strong></p>  
 
 <p><strong><a href="{{ publi.link.url }}">
 <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
 </a></strong></p>  

  <p style="text-align:justify">{{ publi.description }}</p>
  
  <p><em>{{ publi.authors }}</em></p>
  
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  
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


