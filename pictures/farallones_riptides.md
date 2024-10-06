---
title: "Photos"
layout: piclay
excerpt: "COLAB -- Photos"
permalink: /photos/farallones_riptides/
---

<!---->
<!--  Farallon Islands: RIPTIDES students Field Trip -->
<!---->

<hr>
<h3 style="color:Tomato" align="center"> <b>Field Trip to Farallon Islands with RIPTIDES students (September 2017) </b> </h3>
<hr>

<h2><b> (Click [HERE](https://photos.app.goo.gl/FcsToYsxQzCMOd1i1) to see the photo gallery)</b></h2>
{% assign number_printed = 0 %}
{% for pic in site.data.pic_farallones_riptides %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/Gallery/farallones_RIPTIDES/{{ pic.image }}" class="img-responsive" width="100%" style="float: left"/>
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


<div class="container-fluid">
<div class="row">

<div class="col-sm-6">
<div class="container-fluid">
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/Gallery/farallones_RIPTIDES/image1.JPG" class="img-responsive" width="100%" />
<figcaption> Humpback Whale Breach (Photo by Bianca Bahman)
</figcaption>
</figure>
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/Gallery/farallones_RIPTIDES/IMG_9705.JPG" class="img-responsive" width="100%" />
<figcaption> Bloody waters, probably from a seal attacked by a shark (Photo by Bianca Bahman)
</figcaption>
</figure>
</div>
</div>
</div>
</div>


<p> &nbsp; </p>
