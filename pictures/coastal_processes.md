---
title: "Photos"
layout: piclay
excerpt: "COLAB -- Photos"
permalink: /photos/coastal_processes/
---

<br>

<!---->
<!-- coastal processes class -->
<!---->

<hr>
<h3 style="color:Tomato" align="center"> <b>ERTH 434/834 - Coastal Processes Class, Field Trip at San Francisco Bay (October 2017)</b> </h3>
<hr>

<h2><b> (Click [HERE](https://photos.app.goo.gl/0uHhosjR8FLuStwY2) to see the photo gallery)</b></h2>
{% assign number_printed = 0 %}
{% for pic in site.data.pic_coastal_processes %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/Gallery/coastal_processes/{{ pic.image }}" class="img-responsive" width="100%" style="float: left"/>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}

<p> &nbsp; </p>
