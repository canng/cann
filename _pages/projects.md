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
    <p><strong><a href="{{ publi.link.url }}"> <img src="{{ site.url }}{{ site.baseurl }}/images/projectpic/{{ publi.image }}" width="100%" /> </a></strong></p>
    <h3><a href="{{ publi.link.url }}"> <pubtit>{{ publi.title }}</pubtit></a></h3>
    <p>{{ publi.description }}</p>
    <p><em>{{ publi.keywords }}</em></p>
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


