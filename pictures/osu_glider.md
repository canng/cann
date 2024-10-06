---
title: "Photos"
layout: piclay
excerpt: "COLAB -- Photos"
permalink: /photos/osu_glider/
---

<br>

<!---->
<!-- osu glider field work -->
<!---->

<hr>
<h3 style="color:Tomato" align="center"> <b> Glider Research Group - Oregon State University (2009-2014)  </b> </h3>
<hr>

<h2><b> (Click [HERE](https://photos.app.goo.gl/gnOq61buBxv4gSOe2) to see the photo gallery)</b></h2>
{% assign number_printed = 0 %}
{% for pic in site.data.pic_osu_glider %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/Gallery/osu_glider/{{ pic.image }}" class="img-responsive" width="100%" style="float: left"/>
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
