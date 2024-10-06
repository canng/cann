---
title: "Projects"
layout: piclay
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
<a href="{{ publi.link.url }}">
 <div class="well">
 <p><img src="{{ site.url }}{{ site.baseurl }}/images/projectpic/{{ publi.image }}" width="100%" /></p>
 <h3><pubtit>{{ publi.title }}</pubtit></h3>
 <p>{{ publi.description }}</p>
 <p><em>{{ publi.keywords }}</em></p>

 </div>
</a>
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


