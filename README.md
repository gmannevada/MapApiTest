# MapApiTest
www.w3schools.com

#1. Get location lat, longitude:

4. Using the latitude and longitude received from the above GET request, show the user's location on Google Maps. (20 marks)
Reference Video
Reference Content

<script>
var x = document.getElementById("demo");
function getLocation() {
  if (navigator.geolocation) {
    navigator.geolocation.getCurrentPosition(showPosition);
  } else {
    x.innerHTML = "Geolocation is not supported by this browser.";
  }
}

function showPosition(position) {
  x.innerHTML = "Latitude: " + position.coords.latitude +
  "<br>Longitude: " + position.coords.longitude;
}
</script>

<iframe width="600" height="450" frameborder="0" style="border:0"
src="https://www.google.com/maps/embed/v1/place?q=place_id:ChIJdd4hrwug2EcRmSrV3Vo6llI&key=..." 
allowfullscreen></iframe>

#------------------------------
