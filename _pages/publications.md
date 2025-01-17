---
title: "Cann | Publications"
layout: piclay
excerpt: "Publications"
sitemap: false
permalink: /publications/
---


<br>


## Publications

<br>

<img src="{{site.baseurl}}/images/pubpic/cover_publication.png" alt="" />

<br>

<div style="text-align:justify" markdown="1">

<p style="font-size: 18px"><i>For a complete list and updated publications, go to: <a href="https://scholar.google.com/citations?hl=vi&user=xnzuZiAAAAAJ&view_op=list_works&authuser=3&sortby=pubdate"><i class="ai ai-google-scholar-square"></i> Google Scholar</a></i></p>

<br>

<div style="padding: 15px; border: 2px solid transparent; border-color: transparent; margin-bottom: 40px; border-radius: 6px; color: #333333;; background-color: #fcf8e3; border-color: #faebcc;">

<h2>Featured Articles</h2>
<p style="font-size: 18px">
<b><u>Nguyen, C.T.</u></b>, Chidthaisong, A.+, Diem, P.K., Huo, L., 2021. A Modified Bare Soil Index to Identify Bare Land Features during Agricultural Fallow-Period in Southeast Asia Using Landsat 8. Land 10, 1–17. <a href="https://doi.org/10.3390/land10030231"> 10.3390/land10030231</a><a href="{{ site.url }}{{ site.baseurl }}/assets/Article_archive/2021_land_bare_soil_index_mbi.pdf">  <i class="glyphicon glyphicon-file"></i></a> <br>
<br>
<b><u>Nguyen, C.T.+</u></b>, Chidthaisong, A.+, Limsakul, A., Varnakovida, P., Ekkawatpanit, C., Diem, P. K., & Diep, N. T. H., 2022. How do disparate urbanization and climate change imprint on urban thermal variations? A comparison between two dynamic cities in Southeast Asia. Sustainable Cities and Society, 82(July 2022), 103882. <a href="https://doi.org/10.1016/j.scs.2022.103882"> 10.1016/j.scs.2022.103882</a><a href="{{ site.url }}{{ site.baseurl }}/assets/Article_archive/2022_SCS_103822_urban_heat_bkk_hcm.pdf">  <i class="glyphicon glyphicon-file"></i></a> <br>
<br>
<b><u>Nguyen, C. T.+</u></b>, & Chidthaisong A., 2023. Ecosystem Services Provided by Urban Green Spaces in Bangkok Metropolis: Public Awareness and Planning Implications. Urban Ecosystems. <a href="https://doi.org/10.1007/s11252-023-01482-1">10.1007/s11252-023-01482-1</a><a href="{{ site.url }}{{ site.baseurl }}/assets/Article_archive/2023_UE_ESS_UGS.pdf">  <i class="glyphicon glyphicon-file"></i></a>

</p>
</div>

<hr>

<br>

# Research topics

<br>

{% assign number_printed = 0 %}
{% for publi in site.data.publication_list %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
 <h4 style="font-size:18px"><b>{{ publi.title }}</b></h4>
 
 <p><b><img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="50%" /></b>
 
  </p> <p style="font-size:16px">{{ publi.description }}</p>

  <p style="font-size:16px"><em>{{ publi.authors }}</em></p>
  
  <p style="font-size:16px"><b><a href="{{ publi.link.url }}">{{ publi.doi.display }}</a></b></p>

  <p style="font-size:16px"><i class="glyphicon glyphicon-file"></i><b><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></b></p>

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