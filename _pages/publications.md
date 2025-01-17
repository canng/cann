---
title: "Cann | Publications"
layout: piclay
excerpt: "Publications"
sitemap: false
permalink: /publications/
---


<br>

# Research topics

<br>

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
 <h4 style="font-size:20px"><b><a href="{{ publi.link.url }}"><pubtit>{{ publi.title }}</pubtit></a></b></h4>
 
 <p><b><a href="{{ publi.link.url }}">
 <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="90%" />
 </a></b></p> 

  <p style="text-align:justify; font-size:16px">{{ publi.description }}</p>
  
  <p><em>{{ publi.authors }}</em></p>
  
  <p style="font-size:16px"><b><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></b></p>
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


<hr>
<br>

# Projects

<br>

<h2 style="color: #fa7c1e;">On going Projects</h2>

{% assign number_printed = 0 %}
{% for publi in site.data.projectlist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}


<div class="col-sm-6 clearfix">
 <div class="well"> <!--  well-lg >> no box    -->
 <p><a href="{{ publi.link.url }}"> <img src="{{ site.url }}{{ site.baseurl }}/images/projectpic/{{ publi.image }}" width="90%" /> </a></p>
 <a href="{{ publi.link.url }}"> <pubtit>{{ publi.title }}</pubtit></a>
 <p>Period: {{ publi.period }}</p>
 <p>Funder: {{ publi.funder }}</p>
 <p>Keywords: <em>{{ publi.keywords }}</em></p>

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

<br>
<hr>
<br>

<h2 style="color: #fa7c1e;">Past Projects</h2>

{% assign number_printed = 0 %}
{% for publi in site.data.projectlist_past %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}
 

<div class="col-sm-6 clearfix">
 <div class="well"> <!--  well-lg >> no box    -->
 <p><a href="{{ publi.link.url }}"><img src="{{ site.url }}{{ site.baseurl }}/images/projectpic/{{ publi.image }}" width="90%" /> </a></p>
 <a href="{{ publi.link.url }}"> <pubtit>{{ publi.title }}</pubtit></a>
 <p>Period: {{ publi.period }}</p>
 <p>Funder: {{ publi.funder }}</p>
 <p>Keywords: <em>{{ publi.keywords }}</em></p>

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



