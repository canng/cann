---
title: "Cann | Contact"
layout: textlay
excerpt: "Contact me here"
sitemap: false
permalink: /contact/
---




<br>

<div class="container-fluid">
<div class="row">

<div class="col-sm-4">
<div style="text-align:justify" markdown="1">
<p> Dr. Can T. Nguyen <br>
Room 1602, <br>
Environment Centre <br>
Charles University <br>
José Martího 407/2 <br>
160 00 Praha 6 <br>
Czech Republic </p>
<span class="glyphicon glyphicon-phone-alt"></span> (+420) 773-705-812 <br>
<i class="glyphicon glyphicon-envelope"></i> <trongcan.ng@gmail.com>
</div>
</div>

<div class="col-sm-8">
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/contapic/CZP_CUNI.jpg" class="img-responsive" width="500px" height="auto" alt="czp" />
<figcaption> Krystal campus, <span class="copyright">&copy;</span> CZP, CUNI
</figcaption>
</figure>
</div>

</div>
</div>


### Directions to the Environment Centre, Charles University:

<div id="map" style="width:90%;height:500px"></div>

<script>
function myMap() {
  var myCenter = new google.maps.LatLng( 50.094025,14.341628);
  var mapCanvas = document.getElementById("map");
  var mapOptions = {center: myCenter, zoom: 15};
  var map = new google.maps.Map(mapCanvas, mapOptions);
  var marker = new google.maps.Marker({position:myCenter});
  marker.setMap(map);

  var infowindow = new google.maps.InfoWindow({
  content: "Krystal, José Martího 407/2, 162 00 Praha 6-Veleslavín"
});

infowindow.open(map,marker);
}
</script>

<script src="https://maps.googleapis.com/maps/api/js?key=AIzaSyA7i6vSafRzNMdIaq-SslU9oycP9HMR9TM&callback=myMap">
</script>

<br>

