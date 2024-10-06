---
title: "Contact us"
layout: textlay
excerpt: "COLAB -- Contact us."
sitemap: false
permalink: /contact-us/
---

<br>

<div class="container-fluid">
<div class="row">

<div class="col-sm-4">
<div style="text-align:justify" markdown="1">
<p> Dr. Piero Mazzini <br>
Virginia Institute of Marine Science <br>
Post Office Box 1346 <br>
1370 Greate Road <br>
Gloucester Point, VA 23062 </p>
<span class="glyphicon glyphicon-phone-alt"></span> +1 (804) 684-7882 <br>
<i class="glyphicon glyphicon-envelope"></i> <pmazzini@vims.edu>
</div>
</div>

<div class="col-sm-8">
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/contapic/andrews_hall_Malmquist.jpg" class="img-responsive" width="400px" height="auto" alt="andrews" />
<figcaption> Andrews Hall. <span class="copyright">&copy;</span> D. Malmquist.
</figcaption>
</figure>
</div>

</div>
</div>


<div class="container-fluid">
<div class="row">

<div class="col-sm-6">
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/contapic/vims_aereal_2.jpg" class="img-responsive" width="800px" height="auto" alt="VIMS"/>
<figcaption> VIMS Campus <span class="copyright">&copy;</span> VIMS
</figcaption>
</figure>
</div>

<div class="col-sm-6">
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/contapic/C_Katella_VIMS.jpg" class="img-responsive" width="800px" height="auto" alt="rv_virginia" />
<figcaption> R/V Virginia <span class="copyright">&copy;</span> C. Katella
</figcaption>
</figure>
</div>

</div>
</div>




#### Directions to the Environment Centre, Charles University:

<div id="map" style="width:100%;height:500px"></div>

<script>
function myMap() {
  var myCenter = new google.maps.LatLng( 50.094025,14.341628);
  var mapCanvas = document.getElementById("map");
  var mapOptions = {center: myCenter, zoom: 10};
  var map = new google.maps.Map(mapCanvas, mapOptions);
  var marker = new google.maps.Marker({position:myCenter});
  marker.setMap(map);

  var infowindow = new google.maps.InfoWindow({
  content: "1370 Greate Road - Gloucester Point, Virginia"
});

infowindow.open(map,marker);
}
</script>

<script src="https://maps.googleapis.com/maps/api/js?key=AIzaSyA7i6vSafRzNMdIaq-SslU9oycP9HMR9TM&callback=myMap">
</script>

<br>
