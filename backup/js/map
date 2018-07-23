	function initializeMap() {
  console.log('initialize');
  var myOptions = {
    center: new google.maps.LatLng(-7.43027,111.022491),
    zoom: 15,
    mapTypeId: google.maps.MapTypeId.ROADMAP
  };
  var map = new google.maps.Map(document.getElementById("map-canvas"),
    myOptions);

var marker = new google.maps.Marker({
	position: myOptions,
	map: map
});

google.maps.event.addListener(marker, 'click', function() {
	infowindow.open(map,marker);
});

google.maps.event.addDomListener(window, "resize", function() {
	var center = map.getCenter();
	google.maps.event.trigger(map, "resize");
	map.setCenter(center);
	});
}
google.maps.event.addDomListener(window, 'load', initialize);
